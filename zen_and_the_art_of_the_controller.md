---
target: This talk is targeted a newer developers who may or may not have seen their first production project.
track: Junior Track
slides: https://www.slideshare.net/MichaelKelly21/zen-and-the-art-of-the-controller-62823996
presented:
  - [RailsConf 2015](https://www.youtube.com/watch?v=KVkQ9UEQk0Y)
---

# Zen and the Art of the Controller

## Abstract

So you’re fresh out of boot camp or just of a month long binge on RoR tutorials/examples and you’re feeling pretty good about MVC and how controllers fit into the whole framework.  But projects in the wild are often far more complicated than you’ve been exposed to.  In this talk, we’re going to discuss several techniques used by seasoned engineers to build and refactor controllers for features you’ll actually be working on.

## Details

- Introduction and Expectations
- Zen and the Art of the Controller
  - Introduce "Model-less Controllers" Concept
  - Types
    -Static/View Layer Controllers
      - Used to marshal a specific view of data that is oten decoupled from the model domain. These could be:
        - Ajax endpoints
        - Special purpose API endpoints
        - Or simply driven by the visual/site structure of the application
      - Link to OSS examples
      - Code Samples/Local Example
    - Composite Controllers
      - Used when a controller represents an ephemeral "resource" like a session. They tend to control resources that are made up of model data as well as application/user state data.
      - Link to OSS examples
      - Code Samples/Local Example
    - Aggregate Controllers
      - Used to collect data from several different models and data sources to display together. The tend to be used for things like:
        - Dashboards
        - Statistics/Analytics
        - Multi-resource Pages
      - Link to OSS examples
      - Code Samples/Local Examples
- Benefits of these techniques
  - You tie your controller layer to the problem domain you're solving
    - More maintainable for:
      - Debugging/Modifying
      - Navigating/Learning
    - Bugs are also easier to track down when you have many smaller controllers instead of large bloated controllers
  - Allows you to work outside of the rigidity of the framework's theory to develop elegant solutions to specific problems
- Conclusions/Q&A

## Pitch

There is a large generation of new developers who are coming to the craft without a good understanding of the complexity involved in real world projects.  Using controllers that fit this description of a model-less controller is an extremely common practice in Rails development.  Many of the attendees will have used gems like Devise previously without considering the ramifications of its controller structure.  This talk is targeted at new developers looking to expand their knowledge and exposure to real world Rails development.  I have over three years of experience directly with Ruby on Rails and as much mentoring and training new developers.  Juniors read a great deal about MVC and how to design web applications.  But there has always seemed to be some secret sauce to knowing a language/framework syntactically and knowing how to craft it.  In making my own transition from .NET to Rails, I found the myriad of uses for controllers in the gems that I was bundling to be fascinating and extremely valuable to my own design approaches.

