# Add External Exercise

### Integration of External Tools via LTI

The HPI learning platform features many dedicated interactive components for a majority of MOOCs, and we recommend using these native elements if possible. They are supported by our team, have proven to be stable and fit most learners' needs. However, we also offer an interface to connect the HPI learning platform to any other third-party tool to extend the learner's experience with additional, unique features.

### H5P
The option to use the H5P tool for creating external exercises is included by default in all courses.

### Adding an LTI Exercise

<div style="padding:75% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/805427533?h=59f8135ea5&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="openHPI-guidelines-21-LTI.mp4"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Providing an LTI exercise is very similar to the creation of a multiple-choice quiz for the general settings. As the main values are treated similar to a quiz, only LTI specific information are added here.

- Providing a value to `maximal points` is **strongly** recommended. It is required to account points to learners (based on the percentage value provided via LTI) and should only be set to `0.0` (default) if no points can be achieved. The value is not transmitted to the external tool via LTI.
- The `Submission deadline` defines the point in time after which a _new_ launch of the external tool will be handled differently. We recommend mirroring this setting to the external tool (if supported) for the best user experience. The value is not transmitted to the external tool via LTI.
- The `Submission publishing date` is used to reveal the score received through LTI. Depending on the external tool, setting this value does not make sense: If the final score is shown in the external tool, it should also be shown on the HPI MOOC platform immediately. The value is not transmitted to the external tool via LTI.
- Choosing an `LTI provider` is required for an LTI exercise to work. Failing to select a valid LTI provider will break launching the exercise. 
- `Additional parameters for this exercise` enable the Deep Linking to launch specific exercises. This value **is** transmitted to the external tool via LTI. Multiple values can be separated by ampersand `&` and are automatically merged with those values specified for the LTI provider. If a key-value pair is defined for the LTI provider and the exercise, those from the exercise take precedence over those from the provider. The configuration parameters are tool-specific and are defined by the external tool (see the according reference for more details).

### Other Internal LTI Applications

At openHPI, we use some internal applications via LTI:

- [CodeOcean](../../../features/externaltools/codeocean.md) as an educational, web-based execution and development environment for practical programming exercises
- A tool called [TeamBuilder](../../../features/externaltools/teambuilder.md) to create teams based on user preferences.

![HPI Logo](../../../img/HPI_Logo.png)
