# ConstraintLayout
This repository explain about the Google's new released container class, ConstraintLayout as an alternative to LinearLayout and RelativeLayout. 
* In 2016, Google released a new container class, ConstraintLayout
* ConstraintLayout is useful, but it is not required for Android app development, any more than LinearLayout and RelativeLayout are. And, since ConstraintLayout is a library, you will need to take some additional steps to add it to your project, and it adds ~100KB to the size of your Android app. Whether it is worth that extra space and time is for you to decide.
* ConstraintLayout has drag-and-drop GUI builder.
* ConstraintLayout was created with GUI building in mind, to make it a bit easier to infer the right rules based upon where the developer happens to drop a widget.
* WHY ConstraintLayout??
1) Deeper view hierarchies are slower to render than are shallower ones
2) View hierarchies where parents need two passes to size and position their
children are slower to render than are hierarchies where only one pass is needed
* ConstraintLayout is being designed with performance in mind, trying to eliminate as many two-pass scenarios as possible and by trying to eliminate the need for deeply-nested view hierarchies.
* Getting ConstraintLayout

dependencies {

  compile 'com.android.support:support-v13:25.1.1'
  
  compile 'com.android.support.constraint:constraint-layout:1.0.0-beta5'
}
* The ConstraintLayout approach resembles that of the RelativeLayout implementation.
* Attribute
Ex: app:layout_constraintEnd_toEndOf="parent"  (parent to indicate the ConstraintLayout itself)
1) app: is because ConstraintLayout comes from a library, not the Android framework itself
2) layout_ is the standard pre;x for rules based upon a widget’s container, no di:erent than what we saw with the classic containers
3) constraint is used in all the ConstraintLayout-speci;c rule attribute names.
* Guideline:- 
The guideline itself does not appear in the output; it is merely something used at drawing time to aid in drawing. uideline is part of our GUI builder as well, to allow you to visually place the Guideline and connect widgets to that Guideline.
* A Guideline has an orientation, set via android:orientation.
* To define a view's position in ConstraintLayout, you must add at least one horizontal and one vertical constraint for the view. Each constraint represents a connection or alignment to another view, the parent layout, or an invisible guideline.


More About Constraintlayout:-
* https://developer.android.com/training/constraint-layout/index.html
* https://developer.android.com/reference/android/support/constraint/ConstraintLayout.html
* https://codelabs.developers.google.com/codelabs/constraint-layout/index.html?index=..%2F..%2Findex#0
* https://medium.com/exploring-android/exploring-the-new-android-constraintlayout-eed37fe8d8f1
* http://www.journaldev.com/13590/android-constraintlayout
