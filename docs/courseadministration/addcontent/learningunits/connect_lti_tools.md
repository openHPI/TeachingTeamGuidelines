# Connect LTI Tools

### Integration of External Tools via LTI

The HPI learning platform features many dedicated interactive components for a majority of MOOCs, and we recommend using these native elements if possible. They are supported by our team, have proven to be stable and fit most learners' needs. However, we also offer an interface to connect the HPI learning platform to any other third-party tool to extend the learner's experience with additional, unique features.

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/831490139?h=6012d6438f&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="openHPI-guidelines-25-LTI-2"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

#### Usage Scenario

The interface offered by the HPI learning platform is a web-based link technology supporting the access of external educational resources. Opening an external offer through the interface has two main advantages:

- Learners are recognized (with a reduced information set) using a Single Sign-On within the external application. This allows a unified learning experience with the ability to save the current progress and continue on a different device.
- The external tool might return scores for activities back to the course within the HPI learning platform. These are handled similarly to other scores and, depending on the settings, may count towards either the certificate or self-test points.

We recommend using the interface only for interactive, trust-worthy exercises and tools. In order to comply with privacy regulations, non-native LTI providers won't have access to personal user data as part of the Single Sing-On request by default. Especially web links to external resources should not make use of this platform feature and should instead rely on the linking mechanism offered within the rich-text items.

#### Technical requirements

Connecting an external offer requires compliance with a few supported web standards as defined by the MOOC platform. Our interface is based on the [Learning Tools Interoperability](https://www.imsglobal.org/activity/learning-tools-interoperability) standard, to which we will refer as _LTI_ in the following. The LTI standard is one of the most common standards in the area of learning tools and widely adopted within the industry. Many other platforms (such as Moodle or edX for example) also support that. It offers great support for the features required for use cases within the learning environment and provides the two main advantages listed in our [usage scenario](#usage-scenario). LTI uses the [OAuth](https://oauth.net) standard for secure authorization under the hood and support is hence also required. Additionally, a concrete exercise might be accessed through Deep Linking which enables users to start with the given task immediately without clicking through the external offer to find the referenced exercise. Any achieved score can be submitted (and updated) and is transmitted as percentage of the overall score as a float between `0.0` and `1.0`.

Settings of LTI exercises are similar to those of a multiple-choice quiz, e.g. regarding the type, the maximum points or the deadline. We recommend providing as much information as possible and set those if available in both platforms (the MOOC platform and the external tool) for the best user experience.

### Connecting an External Tool with the HPI Learning Platform

Starting an exercise within an external tool requires to simple setup steps:

1. Setting up the LTI provider
2. Creating a course item using a previously set up LTI provider

Splitting the general and item-specific settings, changes (e.g. in the URL of the external tool) can be handled more easily and re-used between different exercises. Thus, it minimizes the setup process for each item. 

#### Linking an LTI Provider

LTI providers are a per-course setting and can be found within the `Course Administration` > `Structure & Content` > `LTI Providers`. Existing LTI providers are shown on the list and can be updated, deleted or supplemented by a new LTI provider. Each LTI provider requires only little information for the setup process. Those are usually defined by the external tool and not know to the HPI MOOC platform. Before setting up an LTI provider, you should familiarize yourself with the required values.

- `Name` and `Description` are only visible for course teachers and administrators and should help you to identify the service.
- The `Launch URL` includes an absolute path for the _LTI endpoint_ (not a specific exercise). Consider the tool's documentation for more details.
- `OAuth consumer key` and `OAuth secret` are required for the authorization management and especially the `OAuth secret` must be kept private! If in doubt, you should exchange the values with new ones. Both values must be equal within the course settings and the external tool itself.
- `Presentation mode` allows the selection between `window`, `pop-up` and `iframe`. Generally speaking, we recommend the `window` setting due to third-party cookie policies. 
  - `window` will launch the external tool in a new window or tab - using the full window space for the content.
  - `pop-up` will launch the external tool in a new pop-up - usually implying smaller windows, a minimized address bar and potential issues with pop-up blockers.
  - `iframe` embeds the content within the HPI learning platform - showing the course navigation and providing only a subset of the available space to the tool. Third-party cookies might be disabled in the learner's browser and hence break cookie-based authentication.
- The `Privacy Mode` specifies which data is passed to the _LTI endpoint_ by each learner accessing the tool. Per default, no personally identifiable information is transmitted to any LTI provider defined in the course context to protect the learners' data. If this setting needs to be adjusted, please contact a platform administrator to discuss further details.
- `Custom fields` are LTI specific parameters and are used in accordance with the LTI standard. Refer to the tool's documentation for more details about the parameters available for use. A common value would be `locale=en` to set the desired language of the external tool to English (if supported).

#### Privacy modes and LTI Provider availability

LTI providers can be set up either per course (local providers) or for the whole platform (global providers). 
Local providers can be set up by course administrators, global providers can only be set up by platform administrators.

The platform allows three different privacy settings:

- **anonymized**: The LTI provider will only obtain an id that is unique for a combination of a user and a course. With this id, the provider is enabled to return the achieved points to the learner's account on the platform and keep track of the learner's action on the connected LTI tool within the current course. The LTI provider is not enabled to access any of the learner's private data and cannot track the learners' actions on the LTI tool across courses. This is the default setting and should only be changed if the requirements for any of the other modes are met.
- **pseudonymized**: The LTI provider will only obtain the cryptographically hashed user_id. With this id, the provider is enabled to return the achieved points to the learner's account on the platform and keep track of the learner's action on the connected LTI tool across courses. The LTI provider is not enabled to access any of the learner's private data. To enable this, a Data Protection Agreement with the provider of the LTI tool is required.
- **unprotected**: user_id, display name and email address are passed to the LTI tool provider. This should only be used for internal LTI tools - meaning LTI tools that are operated by the HPI. Examples are e.g. CodeOcean or the H5P tool that is operated by the HPI (but not e.g. H5P.com). 

As teachers and course administrators do not necessarily know the implications of the privacy settings and the main goal is to protect the learners' privacy, the default privacy setting for local providers is "anonymized". Teachers and course administrators cannot change this setting. If the requirements are fulfilled, platform administrators can change this to a less restrictive mode if this is in the learners' interest or required to improve the overall usability.

Once you put all required values in, you could save the LTI provider and use it in one of the exercises.

### Further Resources

Many educational apps support the LTI standard. The [EduAppCenter](https://www.eduappcenter.com) lists many of the available sites offering an LTI interface. Hence, this page provides a good overview about different examples.

### Selection of External LTI Applications

- [PeerStudio](https://peerstudio.org)
- [GitHub Classroom](https://classroom.github.com)
- [Big Blue Button](https://bigbluebutton.org)
- [Piazza](https://piazza.com/product/lti)

### Developer Resources

- [Learning Tools Interoperability Standard](https://www.imsglobal.org/activity/learning-tools-interoperability)
- [Test LTI Tool for debugging](https://lti.tools/saltire/tp)

![HPI Logo](../../../img/HPI_Logo.png)
