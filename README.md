# Pre-work - *TODOLIST*

**TODOLIST** is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: **Calvin Jian**

Time spent: **3** hours spent in total

## User Stories

The following **required** functionality is completed:

* [X] User can **successfully add and remove items** from the todo list
* [X] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [X] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [ ] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='https://i.imgur.com/x6A5PPA.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

The android development platform is very similar to Swing from Java. Both base their code around Java and have similar layouts. My transition to xml/Android was made very simple due to knowledge of Swing. However, with similarities, I found many differences. In the android development platform, I found the ability to directly put something at some position much more efficient than relying on Layouts and JPanels. For example, in this project, it required two lines to put the add button to the bottom right of the parent and one line to align the editText to the left of the same button. In Swing, I believe I would have to make a new JFrame, give it a layout specific to what I want to do, and then add my objects from first to last. I also found the design tab feature on android studio very helpful. Instead of working purely in xml, the option to use a GUI to introduce features to the app very useful for students when learning how to implement specific things. All in all, I found the android app development platform similar but more useful or efficient compared to Swing.

**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

In this project, ArrayAdapter was used to connect the ArrayList of items with the ListView from the MainActivity.xml. It converts the ArrayList to something that could be shown in the ListView. The adapter is important, because without it, we would need to hardcode how the ListView is displayed and we could not do any of the add/remove/edit to the list. The purpose of 'convertView' in the 'getView' method is a View paramter that can be null. This parameter is then used to call createViewFromResource. In this method, it is checked for null and if it is not null, some variable view is set equal to convertView.

## Notes

Based on the set of videos, some of the instructions are slightly outdated. An example would be the use of compile which is replaced by implementation. I am not 100% certain why this is the case, but there was no need to cast EditText or anything to when using findViewById to the object.

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
