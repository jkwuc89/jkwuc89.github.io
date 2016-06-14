---
layout: post
title: Effectively Documenting a Development Project
---

Over the course of my 26+ year career as a software developer, I've had the opportunity to work on many software projects for several companies. More often than not, I joined a team that was working on a project that started some time ago. When joining an ongoing project, one of the challenges I often faced was getting up to speed and being productive as quickly as possible. What made this significantly more difficult was the lack of good development project documentation. So, how do we solve this? Ultimately, new members are going to be brought on to help with a project. Or in consulting, the project is nearly complete and it is time to transition ongoing development and support of the project to our client. This is where effective development project documentation is an essential tool.

So, what constitutes effective development project documentation? The goal is to get new team members or the client on-boarded and productive with the project as quickly and as painlessly as possible with minimal assistance from current team members. Depending upon the complexity of the project, a good onboarding measurement to shoot for is 1 day. So how does one achieve this goal? Effective project documentation must cover these essentials and it must be as specific as possible. Ambiguity is not a good thing. And strive to limit the choices where possible.

 - Include contact information for all team members and their key responsibilities. This lets everyone know who to contact with questions.
 - What operating system and version is needed? In most cases, development workstations will be provided to team members with the necessary OS.
 - If the project involves mobile development, what mobile devices are needed and where does one request/acquire the devices? Ideally, the necessary hardware will be readily available. 
 - What SDKs and/or JDKs and versions are needed? Include download links.
 - What IDE and version is needed? Again, include a download link. If a license needs to be purchased or acquired before the IDE is downloaded and installed, clearly document how this is done. Ideally, the necessary licenses will already be purchased and ready to use.
 - How is the IDE configured to conform to project development standards? Every modern IDE has export functionality that allows settings to be exported and then, imported. Leverage this to make IDE configuration that conforms to the standards practically foolproof.
 - What version control system is being used and how is access to it requested? The popular choices are Git, Subversion and CVS. Include any contact information and/or instructions required to request access. Ideally, access to version control will be set up prior to onboarding.
 - What version control client software and version is needed? Remember those download links.
 - What build tool software and version is needed? Some IDEs like Xcode do not require separate build tool software. Some do. Examples include Ant, Maven and Gradle. Don't forget those download links. Also include any step by step instructions required to install the build tool software because nearly every build tool requires some OS specific configuration to be done.
 - What dependency management server is used and how is access to it requested? Build tools like Maven and Gradle depend upon a dependency management server to download the necessary dependencies to build a project. And most corporations concerned with software licensing host a dependency management server in house to control what libraries can be used to develop and build projects. Include any step by step instructions required to configure the IDE and/or build tools to use the dependency management server.
 - Once everything above installed and configured, how is the project pulled from source control, built, tested, installed/deployed and executed? Provide repeatable step-by-step instructions.
 - What standards and/or guidelines are followed when developing, testing, and committing changes?
 - Include an FAQ section that includes answers to commonly encountered questions or problems.

Over time, project changes will require changes to the project documentation. So, make sure that the project documentation is always kept up to date.

When teams spend the time to effectively document their project as described above, it enables effective and efficient onboarding of and knowledge transfer to new team members and clients which allows them to get to the business of being productive as quickly as possible.