---
name: 'Testing overview'
about: 'This is used by the DataCamp Projects team and should not be used by instructors.'

---

Hi, @______! Here is some help for completing the tests:

### Overview of testing

Testing for R projects is done using Hadley Wickham's `testthat` package. There's a nice overview of how to use it under the "testthat package" heading in this ["Writing tests" blog post](http://kbroman.org/pkg_primer/pages/tests.html). Here's a key bit of that post:

<img width="694" alt="screenshot 2018-09-08 00 35 02" src="https://user-images.githubusercontent.com/15305603/45247355-0ed45080-b2ff-11e8-9954-90c062ef4997.png">

### Details of testing

The testing chapter in the _R packages_ book gets into the details, along with workflow advice and concrete examples: http://r-pkgs.had.co.nz/tests.html

### Testing for projects

For DataCamp projects, we don't need to and can't possibly test _everything_. We just need to give students some help along the way. It is difficult/impossible to test things not saved to objects and cells with multiple plots. And that's okay.

I'm going to attach a model project example for you to peruse. [Functions for Food Price Forecasts](https://drive.google.com/open?id=1S32FBNVxBwAZOJZq0yIL6KLYm0esYzkS). Note that this project was written by DataCamp's Content Quality Lead, Richie Cotton. Richie also wrote a book called [Testing R Code](https://www.crcpress.com/Testing-R-Code/Cotton/p/book/9781498763653) so he knows his stuff! Take special note that each failed test message mentions the specific piece of code that was tested, which ensures the student knows _why_ their code was marked incorrect.

Please dig into this and let me know if you get stuck.

### Testing your tests

Ensure your tests pass in your local environment by processing a solution code cell then its tests back to back. Here's a video of me demo-ing that for another instructor:

https://www.useloom.com/share/1dc647f7b58340cfa7adcadf5244937b

Ensure your tests pass in the DataCamp environment by inspecting your Project's `develop` branch's build log, which is in the first link in this GitHub repo's `README.md`. If tests pass locally but not on DataCamp, there is likely an issue with the installations in `requirement.R`. Try to fix it yourself, then reach out to me if you're stuck (this happens fairly often as some of the installation info is removed from the view of instructors).
