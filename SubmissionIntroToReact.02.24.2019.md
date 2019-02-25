# **Exercises**
## **Submit answers to the following questions:**

#### 1. In your own words, explain React's **Virtual DOM.** What gives React its fast performance?

I can remember years ago when it took seconds to refresh a web page. Today refreshing a webpage still takes time depending upon the complexity of the website. So to save time refreshing or rewriting the web page should be avoided as much as possible. In my opinion this is the approach React developers took when building react. DOM manipulation is the heart of the modern, interactive web. Unfortunately it is also a lot slower than most JavaScript operations. This slowness is made worse by the fact that **most JavaScript frameworks update the DOM much more than they have to.**  As an example, let's say that you have a list that contains ten items. You check off the first item. Most JavaScript frameworks would rebuild the entire list. That's ten times more work than necessary! Only one item changed, but the remaining nine get rebuilt exactly how they were before.

Rebuilding a list is no big deal to a web browser, but modern websites can use huge amounts of DOM manipulation. Inefficient updating has become a serious problem.

To address this problem, the people at React popularized something called the *virtual DOM.*

The Virtual DOM
In React, for every DOM object, there is a corresponding "virtual DOM object." A virtual DOM object is a representation of a DOM object, like a lightweight copy.

A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing's power to directly change what's on the screen.

Manipulating the DOM is slow. Manipulating the virtual DOM is much faster, because nothing gets drawn onscreen. Think of manipulating the virtual DOM as editing a blueprint, as opposed to moving rooms in an actual house.

How it helps
When you render a JSX element, every single virtual DOM object gets updated.

**This sounds incredibly inefficient, but the cost is insignificant because the virtual DOM can update so quickly.**

Once the virtual DOM has updated, then React compares the virtual DOM with a virtual DOM snapshot that was taken right before the update.

By comparing the new virtual DOM with a pre-update version, React figures out exactly which virtual DOM objects have changed. This process is called "diffing."

Once React knows which virtual DOM objects have changed, then React updates those objects, and only those objects, on the real DOM. In our example from earlier, React would be smart enough to rebuild your one checked-off list-item, and leave the rest of your list alone.

This makes a big difference! React can update only the necessary parts of the DOM. React's reputation for performance comes largely from this innovation. **This is the key to React's fast performance.**

In summary, here's what happens when you try to update the DOM in React:

The entire virtual DOM gets updated.
The virtual DOM gets compared to what it looked like before you updated it. React figures out which objects have changed.
The changed objects, and the changed objects only, get updated on the real DOM.
Changes on the real DOM cause the screen to change.



#### **2. In your own words, describe React's core concept of uni-directional data flow. Draw diagrams to illustrate. Discuss the answer with your mentor in your next session.**


In my own words data can flow in only one direction in React. This means that data has one, and only one way to be transferred to other parts of the application.

In React this means that:
* state is passed to the view and to child components
* actions are triggered by the view
* actions can update the state
* the state change is passed to the view and to child components

In the below illustration data is flowing only in a clockwise direction ... this illustrates uni-directional data flow.

                .   .  .
             .            .
         .                   .
     view                     actions
       .                        .
         ,                    .
           .  .  state  .  .
  