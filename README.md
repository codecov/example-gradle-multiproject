# [Codecov][1] Gradle Example

1. Add Jacoco Plugin to your `build.gradle`. [See here](https://github.com/codecov/example-gradle/blob/master/build.gradle#L5)
1. Set Jacoco to export xml. [See here](https://github.com/codecov/example-gradle/blob/master/build.gradle#L18-L23)
1. Execute your tests as normal
1. Call `gradle codeCoverageReport` to generate report. [See here](https://github.com/codecov/example-gradle/blob/65f88382659cf17c8693c3079941a12c8d004f03/circle.yml#L3)
1. Call `bash <(curl -s https://codecov.io/bash)` to upload reports to Codecov. [See here](https://github.com/codecov/example-gradle/blob/65f88382659cf17c8693c3079941a12c8d004f03/circle.yml#L4)
  - Public project? Using TravisCI, CircleCI or AppVeyor? You're all set! No upload token required.
  - Otherwise please include your repository upload token. [See here](http://docs.codecov.io/v4.3.0/docs/about-the-codecov-bash-uploader#section-upload-token)

