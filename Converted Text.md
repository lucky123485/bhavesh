# ![](https://lh7-us.googleusercontent.com/dq0BJODWYT0B8pjctYJja7M2rsdOqR9CIVh-6Mq5svxso0hwg9Em5owMZyqHAaqSvoPjaAX8FH2L7tbV6XXLi0Nq0GTX1Q8Rj7LRqFZ2GsPdfsPTFKmVC_c8Lmu1aOkv33JFGVsnFgm-HoCON3qVJ-Y)

# Cucumber - Overview

Cucumber is a testing tool that supports Behaviour Driven Development (BDD) framework. It defines application behaviour using simple English text, defined by a language called Gherkin.

Cucumber allows automation functional validation that is easily read and understood. Cucumber was initially implemented in Ruby and then extended to the Java framework. Both the tools support native JUnit.

**What is Cucumber Framework?**

Cucumber Framework executes automated acceptance tests written in the “Gherkin” language. Gherkin is a domain-specific language for behaviour descriptions. Gherkin is business-readable.

Cucumber test automation makes use of two important files:

- **Feature file –** Contains code written in Gherkin (plain English text)
- **Step definition file –** Contains the actual code written by the developer

Cucumber acts as a bridge between the following teams:

- Business Analysts and Software Engineers
- Manual and Automation Testers
- Manual Testers and Developers


# Benefits of using Cucumber Testing Tools

- Testers can write Test scripts without having in-depth knowledge of programming
- Plugins are faster as compared to Selenium
- Supports various programming languages
- Code can be reused
- Simple and quick setup
- Flexible with different software platforms like Selenium, Ruby on Rails, Watir, Spring framework, and so forth


# How does Cucumber work?

Cucumber BDD framework mainly consists of three major parts:

- **Feature File:** Cucumber tests are written in plain text files called feature files stored with the extension – “.feature”. A Feature File can be described to make the documentation more legible. These files describe the behaviour and functionality of the software using a specific syntax called Gherkin. Gherkin is a structured language that uses keywords like Given, When, and Then to define the steps of a test scenario.
- **Step Definitions:** Each step in a feature file is associated with a step definition implemented in the code. Step definitions define the actions or operations that must be executed for each step of the test scenario. They map the plain text steps in the feature file to the corresponding code implementation.
- **Test Runner File:** In Cucumber, the test runner file executes the Cucumber feature files and coordinates the steps defined in those feature files with the corresponding step definitions.


### Example of Cucumber Test

Here’s an example of the Cucumber Test for checking the Login functionality for an existing user.

Scenario: As an existing user, I want to log in successfully.

Given:the user is on the Home page

When:the user navigates to the Login page

And:the user enters the username and password

Then:the successful login message is displayed


# BDD in Cucumber Automation

The behaviour-driven development’s approach involves the usage of shared language that enhances communication between various tech and non-tech teams. Tests are more user-focused and based on the system’s behaviour. In BDD, “Given-When-Then” is the proposed approach for writing test cases.

Consider the example below for a better understanding:

- Given the user has entered invalid credentials
- When the user clicks the submit button
- Then display the proper validation message


# Benefits of BDD in Cucumber Framework

- Focuses on defining ‘behaviour’ rather than defining ‘tests’
- Enhances communication among the members of a cross-functional product team
- Helps reach a wider audience by the usage of non-technical language
- It enables you to understand how the system should perform from the developer’s and customer’s perspective
- The improvement in the quality of code results in reduced costs of maintenance and also minimizes the project’s associated risks.


# Limitations of Behavior-driven development

- Testers must have prior experience in [TDD (Test-driven Development)](https://www.browserstack.com/guide/what-is-test-driven-development) to work in BDD
- BDD approach may be ineffective if the requirements are not correctly analysed
- Testers must have sufficient technical skills


# Software tools supported by Cucumber

The piece of code to be executed for testing may belong to different software tools like **Selenium**, **Ruby on Rails**, etc. But cucumber supports almost all popular software platforms, and this is the reason behind Cucumber's popularity over other frameworks such as **JDave**, **Easyb**, **JBehave**, etc. Some Cucumber supported tools are given below:

Ruby on Rails

- Selenium
- PicoContainer
- [Spring Framewo](https://www.javatpoint.com/spring-tutorial)rk
- Watir


## Which language is used in cucumber?

**Cucumber** tool was originally written in the "**Ruby**" programming language. It was exclusively used only for testing of Ruby as a complement to the **RSpec** BDD framework.

But now, Cucumber supports a variety of different programming languages including Java, JavaScript, PHP, Net, Python, Perl, etc. with various implementations. In Java, it supports **native JUnit**.

![](https://lh7-us.googleusercontent.com/lzitEW5ehCSF_PYKiGSH_08eINNYDHsqHiU2Aa8CutNgQ15QMd9MsX8rJQ457EIKDGrHrdjvYoz3v8xQ_VI28TSC0e6mMQZYDRfK5cslKDEY2Gbsiacw8MMLNpBOsZoBAZHTRZfO54W8h3wQwiVKYOM)

**What is Gherkin?**

Gherkin is Cucumber’s language parser, which allows software behaviours to be specified in a logical language that people can understand. This means that Cucumber feature documentation is written in business-facing text that is non-technical and human readable for stakeholders like business analysts and managers. This is achieved because Gherkin’s natural language syntax is designed to provide easy to understand documentation of the code under test. Gherkin is written in a syntax that supports BDD.

‍

**How does Gherkin work?**

Cucumber tests are divided into ‘Features’, which are use cases that describe a specific function being tested.

These ‘Features’ are further divided into ‘Scenarios’, which describe a flow of events and map 1 to 1 with an executable test case for the system. ‘Features’ often have multiple ‘Scenarios’

“Scenarios’ are defined by a series of ‘Steps’ which describe the flow in preconditions, actions, and results in keywords such as; Given, When, Then, And, and But.

### important Terms used in Gherkin

- Feature
- Background
- Scenario
- Given
- When
- Scenario Outline Examples


### Feature:

The file should have extension .feature and each feature file should have only one feature. The feature keyword being with the Feature: and after that add, a space and name of the feature will be written.


### Scenario:

Each feature file may have multiple scenarios, and each scenario starts with Scenario: followed by scenario name.


### Background:

Background keywords help you to add some context to the scenario. It can contain some steps of the scenario, but the only difference is that it should be run before each scenario.


### Given:

The use of the Given keyword is to put the system in a familiar state before the user starts interacting with the system. However, you can omit writing user interactions in Given steps if Given in the “Precondition” step.

**Syntax:**

Given

Given - a test step that defines the 'context

Given I am on "/."


### When:

When the step is to define action performed by the user.

**Syntax:**

When

A When - a test step that defines the 'action' performed

When I perform "Sign In."


### Then:

The use of ‘then’ keyword is to see the outcome after the action in when step. However, you can only verify noticeable changes.

 **Syntax:**

Then

Then - test step that defines the 'outcome.'

Then I should see "Welcome Tom."


### And & But

You may have multiple given when or Then.

**Syntax:**

But

A But - additional test step which defines the 'action' 'outcome.'

But I should see "Welcome Tom."

And - additional test step that defines the 'action' performed

And I write  "EmailAddress" with "Tomjohn\@gmail.com."

Given, When, Then, and, but are test steps. You can use them interchangeably. The interpreter doesn’t display any error. However, they will surely not make any ‘sense’ when read.

**Gherkin Examples**


Feature:  Login functionality of social networking site Facebook. 

Given:  I am a facebook user. 

When: I enter username as username. 

And I enter the password as the password 

Then I should be redirected to the home page of facebook 

The scenario mentioned above is of a feature called user login.

All the words written in bold are Gherkin keywords.

Gherkin will analyse each step written in the step definition file. Therefore, the steps are given in the feature file and the step definition file should match.


## Best practices of using Gherkin

- Each scenario should execute separately
- Every feature should able to be executed along
- Steps information should be shown independently
- Connect your Scenarios with your requirements
- Keep a complete track of what scenarios should be included in a requirement document
- Create modular and easy to understand steps
- Try to combine all your common scenarios


##     Advantages of Gherkin

- Gherkin is simple enough for non-programmers to understand
- Programmers can use it as a very solid base to start their tests
- It makes User Stories easier to digest
- Gherkin script can easily understand by business executives and developers
- Gherkin Testing targets the business requirements
- A significant proportion of the functional specifications is written as user stories
- You don’t need to be expert to understand the small Gherkin command set
- Gherkin Test cases link acceptance tests directly to automated tests
- Style of writing tests cases are easier to reuse code in other tests

       Disadvantages of Gherkin

- It requires a high level of business engagement and collaborations
- May not work well in all scenarios
- Poorly written tests can easily increase test-maintenance cost


### Cucumber with Selenium

Many organisations prefer the Selenium framework for cross-browser compatibility testing. These organisations also prefer integrating Cucumber with Selenium as it makes it easier to read and understand the flow of applications among the members of different teams. Gherkin syntax involves simple and plain text, which makes it easier to understand test cases

- Running the Cucumber Selenium tests on real browsers and devices is essential.
- Since
- BrowserStack cloud testing supports [Selenium testing with Cucumber](https://www.browserstack.com/guide/automation-using-cucumber-selenium); sign up, choose the required device-browser-OS combination, and start testing websites.
- With [BrowserStack Test Management](https://www.browserstack.com/test-management), teams can upload BDD-JSON based report upload using Cucumber. This enables you to sync test case reports on BrowserStack Test Management from your terminal.

**Summary**

- The Cucumber testing tool is a purely business-driven development tool written in Ruby.
- The business-driven development approach is an advancement over the test-driven development approach, which follows the
- ‘Given-When-Then’ steps for writing test cases
- Cucumber framework uses Gherkin ( A simple plain text language parser) to describe expected software behaviours logically, resulting in better communication and collaboration among technical and non-technical team members.
- Cucumber is compatible with popular software platforms like Selenium, Watir, Ruby, and others.
- One must also consider the limitations before deciding on the behaviour-driven development approach.
