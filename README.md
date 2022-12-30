Shared ViewModel Across Fragments
=================================

This app contains an order flow for cupcakes with options for quantity, flavor, and pickup date.
The order details get displayed on an order summary screen and can be shared to another app to
send the order.

This app demonstrates multiple fragments in an activity, a shared ViewModel across fragments,
data binding, LiveData, and the Jetpack Navigation component.


https://developer.android.com/courses/pathways/android-basics-kotlin-unit-3-pathway-4



Summary
--------------
* The ViewModel is a part of the Android Architecture Components and the app data saved within the ViewModel is retained during configuration changes. To add a ViewModel to your app, you create a new class and extend it from the ViewModel class.

* Shared ViewModel is used to save the app's data from multiple fragments in a single ViewModel. Multiple fragments in the app will access the shared ViewModel using their activity scope.

* LifecycleOwner is a class that has an Android lifecycle, such as an activity or a fragment.

* LiveData observer observes the changes to the app's data only if the lifecycle owner is in active states (STARTED or RESUMED).

* Listener bindings are lambda expressions that run when an event happens such as an onClick event. They are similar to method references such as textview.setOnClickListener(clickListener) but listener bindings let you run arbitrary data binding expressions.

* The LiveData transformation method(s) provides a way to perform data manipulations on the source LiveData and return a resulting LiveData object.

* Android frameworks provides a class called SimpleDateFormat, a class for formatting and parsing dates in a locale-sensitive manner. It allows for formatting (date → text) and parsing (text → date) dates.

* Android keeps a back stack of all the destinations you've visited, with each new destination being pushed onto the stack.

* By tapping the Up or Back button, you can pop destinations off the back stack.

* Using the Jetpack Navigation component helps you push and pop fragment destinations off the back stack, so that the default Back button behavior comes for free.

* Specify the app:popUpTo attribute on an action in the navigation graph, in order to pop destinations off the back stack until the specified one in the attribute value.

* Specify app:popUpToInclusive="true" on an action when the destination specified in app:popUpTo should also be popped off the back stack.

* You can create an implicit intent to share content to an email app, using Intent.ACTION_SEND and populating intent extras such as Intent.EXTRA_EMAIL, Intent.EXTRA_SUBJECT, and Intent.EXTRA_TEXT to name a few.

* Use a plurals resource if you want to use different string resources based on quantity, such as the singular or plural case.

* Learned how to set up a LiveData test.

* Learned how to test LiveData itself.

* Learned how to test LiveData that is transformed.

* Learned how to observe LiveData in a unit test.


