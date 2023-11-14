# Class 34

## How are releases and versioning related?

Releases and versioning are closely related in the app development process. When you release an app, you are essentially making a specific version of your application available to users. Versioning is the practice of assigning unique identifiers (usually in the form of version numbers) to different releases of your app. Each release represents a set of changes, improvements, or new features, and versioning helps users and developers track and understand the evolution of the app over time.

---

## What are the 5 main tasks you need to complete to prepare your application for release to the Google Play Store?

1. Configure your app for release:

- Disable and remove logging.
- Set debuggable to false in Groovy or isDebuggable to false in Kotlin script.
- Set app's version information.

2. Build and sign a release version of your app:

- Use Gradle build files with the release build type to build and sign the app.

3. Test the release version:

- Thoroughly test the release version on at least one target handset device and one target tablet device.
- Utilize tools like Firebase Test Lab for testing across various devices and configurations.

4. Update app resources for release:

- Ensure all app resources, such as multimedia files and graphics, are updated and included with the app or staged on production servers.

5. Prepare remote servers and services:

- Ensure external servers or services your app depends on are secure and production-ready.

Additional tasks may include creating an account on the app marketplace (Google Play), creating promotional materials like screenshots and videos, configuring marketplace settings, and finally, publishing the app for download by users.

---

## Things I want to know more about

- Google Play Publishing Process