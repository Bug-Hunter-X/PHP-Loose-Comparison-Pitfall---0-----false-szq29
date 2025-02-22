# PHP Loose Comparison Pitfall: '0' == false

This repository demonstrates a common pitfall in PHP programming related to loose comparison (`==`) and unexpected type juggling. The example shows how comparing a string '0' with a boolean `false` evaluates to `true` due to PHP's loose type system. This can lead to unexpected behavior and difficult-to-debug issues in applications.

## Bug Description
The `bug.php` file contains code that showcases the issue. The comparison `'0' == false` evaluates to `true`, which is often not the intended behavior.  This is because PHP converts `false` to 0 for the comparison.

## Solution
The `bugSolution.php` file demonstrates the correct way to perform the comparison using strict comparison (`===`), which ensures both value and type are checked, preventing the unexpected outcome. 

## How to Run
1. Clone this repository.
2. Run `php bug.php` and `php bugSolution.php` from your terminal to observe the different behaviors.
