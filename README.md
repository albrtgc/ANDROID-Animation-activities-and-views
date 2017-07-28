# ANDROID-Animation-activities-and-views

Create four files for the four types of animations

## Slide from left

<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate 
        android:fromXDelta="-100%p" 
        android:toXDelta="0"
        android:interpolator="@android:anim/accelerate_decelerate_interpolator"
        android:duration="2000"/>
</set>

## Slide from right

<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate 
				android:fromXDelta="100%p" 
				android:toXDelta="0"
        android:interpolator="@android:anim/accelerate_decelerate_interpolator"
        android:duration="2000"/>
</set>

## Slide to left

<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate 
				android:fromXDelta="0" 
				android:toXDelta="-100%p"
        android:interpolator="@android:anim/accelerate_decelerate_interpolator"
        android:duration="2000"/>
</set>

## Slide to right

<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate 
				android:fromXDelta="0" 
				android:toXDelta="100%p"
        android:interpolator="@android:anim/accelerate_decelerate_interpolator"
        android:duration="2000"/>
</set>

To use the animations, we must to override the animations after to start or finish activities.

-> overridePendingTransition(R.anim.slide_from_left, R.anim.slide_to_right);
- First parameter is enter animation.
- Second parameter is exit animation.
