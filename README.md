gproj-web-workspace
===================

Workspace and source tree for GProj web resource management


> **NOTE**: The script POST-CHECKOUT.sh is provided as a utility for use
>  after cloning this source tree. The script will ensure that all
>  submodules are retrieved, recursively, and will set each primary
>  submodule to the 'master' branch.

## Sidebars

### Common Tasks - Task Definitions

The following outlines represent a series of _task definitions_ for
some common activities within the `gproj-web-workspace` project.

#### Activity: Create a New Project in This Work Area

1. Create _source repository_ (at GitHub, typically)
2. Add _source tree_ as a _submodule_ of the `gproj-web-workspace`
   _source tree_
3. Add Maven _POM_ to _source repository_
4. Modify the _POM_ `${PARENT_DIR}/pom.xml`, so as to ensure that
   the new _POM_ will be denoted (directly or indirectly) as a Maven
   _module_ of the _root POM_ in this workspace (directly, a a Maven
   _module_ of its most directly _containing POM_. This step is
   neccessary for the purpose of maintaining _project structure_,
   within the _workspace_, whether or not the new _POM_ may denote the
   _root POM_ in this workspace as its _parent POM_ (as it may not, in
   the case of a _third party project_ being added to this _source
   tree_)

#### Steps: Develop a New Project in This Work Area

1. _Import_ the new _source tree_ as a _project_ in the
   [Eclipse IDE][eclipse], using the
   [Maven Integration for Eclipse][m2e]
2. _Develop content for the project_. (This is an _abstract step_. The
   composition of the _tools and deliverables configuration_ for the
   completion of this task, as a _class definition_, would derive from
   the goals and the nature of the project)

[eclipse]: http://www.eclipse.org/
[m2e]: http://wiki.eclipse.org/M2E
