# Read 38

## Intent Filters

1. What are the three criteria an acticity’s intent filter must fulfill in order for a system to send an intent to that activity?

An activity's intent filter must fulfill the following three criteria for the system to send an intent to that activity:

- Action: It specifies the action to perform, such as ACTION_SEND or ACTION_VIEW.
- Data: It describes the data associated with the intent, which can include MIME type, URI prefix, or URI scheme.
- Category: It provides additional characterization of the activity handling the intent, usually related to user gesture or location.

2. How does an activity retrieve the Intent that it was started by?

An activity retrieves the Intent that started it by calling getIntent() during the early callbacks, such as onCreate() or onStart(). This allows the activity to examine the Intent and determine the action and data associated with it.

3. Explain intents to a non-technical friend.

Intents are like requests or messages that apps use to communicate with each other. Imagine you have different apps on your phone, and sometimes you want them to work together. Intents are like notes with specific instructions that one app can send to another, telling it to perform a certain action, like sharing a photo or opening a link. It's a way for apps to collaborate and make your overall experience smoother and more connected.

---

## Implicit vs. Explicit Intents

1. Compare and contrast implicit and explicit intents.

**Explicit Intents:**

- Usage: Explicit intents are used when you know which component (activity, service, etc.) you want to launch.
- Target Component: You explicitly specify the target component in the intent, providing the class name or component name.

Example Code:
`Intent explicitIntent = new Intent(CurrentActivity.this, TargetActivity.class); startActivity(explicitIntent);`

**Implicit Intents:**

- Usage: Implicit intents are used when you want the system to determine the appropriate component to fulfill the request.
- Action or Category: Instead of specifying a class name, you define an action or category, and the system resolves the intent to the appropriate component that can handle it.

Example Code:
`Intent implicitIntent = new Intent(Intent.ACTION_VIEW, Uri.parse("https://www.example.com")); startActivity(implicitIntent);`

**Comparison:**

- Explicit: You have a specific target in mind.
- Implicit: You let the system find the suitable component based on the defined action or category.

2. What is the primary information contained within an Intent?

- Action: Describes the type of operation to be performed 
- Data: Specifies the data on which the action should be performed 
- Type: Defines the MIME type of the data
- Component: For explicit intents, this specifies the target component 
- Extras: Additional information packaged as key-value pairs 

---

## Things I want to know more about

- Intent Filters and Priority

- Dynamic Intent Handling