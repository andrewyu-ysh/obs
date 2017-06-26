# obs - Automatic Identification and Analysis of Basketball Plays

This repository is a placeholder for my Master's Thesis project, which was submitted in partial fulfillment of the requirements for the degree: Master of Computer and Information Science. The thesis was successfully defended on May 8, 2017. For the abstract, please visit http://rave.ohiolink.edu/etdc/view?acc_num=csu14943636475232. For more details about the project and other inquiried, contact me at andrewyu.ysh@gmail.com.

## What does the project do?

The thesis describes methods to _create an end-to-end framework that visualizes and automatically identifies basketball plays, specifically on-ball screens_. Modules in the framework include data collection, preprocessing, visualization, and analysis using player motion-tracking data captured from high-speed cameras in NBA arenas.

## What it an On-Ball Screen (OBS)?

The on-ball screen involves four players, two on defense guarding two on offense, one of which is holding the ball.

<p align="center">
    <img src="https://github.com/andrewyuysh/obs/blob/master/img/obs.jpg" width="750">
</p>

First, the offensive player without the ball (screener) stands still and “sets a screen”, effectively making himself an obstacle for anyone trying to move through his area (Figure 1.1).

Then, the offensive player with the ball (ball-handler) approaches and brushes by the screener. The defensive player trying to stay close to the ball-handler will have his path blocked by the screener, putting him in a poor position to defend the ball-handler (Figure 1.2).
While the defender struggles to recover by going around the screen, another defender (usually the one guarding the screener) must step up to defend the ball-handler (Figure 1.3).

In the end, a different defender is guarding the ball-handler and a “switch” has occurred (Figure 1.4). The switch refers to the fact that two defenders have switched places in guarding their opponents. Often, the goal of the on-ball screen is to force a poor defender to defend a good offensive player.

The on-ball screen is a simple play that is fundamental to any NBA offense, from which a variety of different plays, like the pick-and-roll, can arise. To defend against it, a team must define a set of rules to follow when facing an on-ball screen, allowing defenders to coordinate properly and respond quickly. These rules are often the defining philosophy of a defensive-minded coach, and a great defender follows them instinctively.

## What do the visualizations look like?

<p align="center">
    <img src="https://github.com/andrewyuysh/obs/blob/master/img/court-viz.png" width="750">
</p>

## Tell me more about the framework

<p align="center">
    <img src="https://github.com/andrewyuysh/obs/blob/master/img/pipeline-2-expand-redact.png">
</p>

The data flow pipeline has five layers, starting with Data Gathering. Black nodes on the right side indicate the completion of one layer; if such nodes are intermediary, they are redrawn as inputs to the next layer in grey. Round-edge rectangular nodes refer to distinct functions in the pipeline, folded rectangles refer to web-based data sources, and cylinders refer to organized data stores. Diamonds are the end-products of the pipeline.

## Will you share your code or give more details on the framework?

Probably not, but feel free to contact me at andrewyu.ysh@gmail.com with any questions.
