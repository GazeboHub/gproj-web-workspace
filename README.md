gproj-web-workspace
===================

Workspace and source tree for GProj web resource management

> **Planning Note**: Since the last subsantial update of the [gproj-web-workspace](https://github.com/GazeboHub/gproj-web-workspace) the Gazebo Project's web development plans have been revised, such that OpenShift will not be used as a host for a Java web portal service -- the Gazebo Project then preferring [Digital Ocean](https://www.digitalocean.com/) for VPS hosting of a Glassfish application server, in a Glassfish/Liferay bundle. This change is made primarily in consideration of budgetary concerns, as in regards to the projected cost of a fully scaled Java web portal framework application at OpenShift, compared to pricing for comparable resources in Digital Ocean hosting. Secondly, a VPS host account at Digital Ocean would provide a much wider range for service configuration and service control methods. This change in the project's hosting plan has not yet been reflected in structure of the Gazebo Project web workspace.


> **Developers Note**: The script POST-CHECKOUT.sh is provided as a utility for use
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
