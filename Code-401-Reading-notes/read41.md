[Allowing Other Apps to Start Your Activity](https://developer.android.com/training/basics/intents/filters)


If your app can perform an action that might be useful from another app, your app should be prepared to respond to action requests by specifying the appropriate intent filter in your activity.

For example, if you build a social app that can share messages or photos with the user's friends, you should support the ACTION_SEND intent. Then, when users initiate a "share" action from another app, your app appears as an option in the chooser dialog (also known as the "disambiguation dialog"),


- In order to properly define which intents your activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.
- The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:
  - Action : A string naming the action to perform.
  - Data : A description of the data associated with the intent.
  - Category : Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it’s started.
- Each incoming intent specifies only one action and one data type, but it’s OK to declare multiple instances of the <action>, <category>, and <data> elements in each <intent-filter>.


### Return a Result 
- simply call setResult() to specify the result code and result Intent.
- When your operation is done and the user should return to the original activity, call finish() to close (and destroy) your activity.
- You must always specify a result code with the result.
- If you simply need to return an integer that indicates one of several result options, you can set the result code to any value higher than 0.
- If you use the result code to deliver an integer and you have no need to include the Intent
- you can call setResult() and pass only a result code.