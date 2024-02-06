# Google Summer Of Code 2024 for Casdoor

## What is Google Summer Of Code?

Google Summer of Code (GSoC) is a global program held by Google to bring students into open source software development. Students work with an open source organization on a 3 month programming project during their break from school. See more details at: https://summerofcode.withgoogle.com/

## How we select students:

The student will be more likely selected if he/she:

1. Contribute to Casdoor related project before.
2. Familiar with the techniques required by the idea he selected.
3. Show the previous code related to the idea on personal website or GitHub.
4. Provide a personal website and descriptions for previous work/projects.
5. Provide demo sites for the previous projects if possible.
6. Provide a resume/CV.

## Get started

1. Choose an idea from our list: https://github.com/casdoor/SummerOfCode2024
2. Send your resume/CV in PDF to: admin@casdoor.org
3. Do a self-introduction in: https://discord.gg/PD9g8wE6X9
4. Get familiar with the existing code, try to solve opened issues for your chosen idea's repo before & after application deadline.
5. If you have questions, you can ask the mentor of the idea via GitHub or [Discord](https://discord.gg/PD9g8wE6X9).
6. Submit your proposal in [GSoC official site](https://summerofcode.withgoogle.com/). The deadline is TBD.

## Ideas

- [Casdoor Core Engine (Golang)](#casdoor-core-engine-golang)
- [Casdoor](#casdoor)
- [Casnode](#casnode)
- [Casdoor Dashboard](#casdoor-dashboard)
- [Casdoor for C/C++](#casdoor-for-cc)
- [Casdoor for Java](#casdoor-for-java)
- [Casdoor for .NET](#casdoor-for-net)
- [Casdoor for .NET](#casdoor-for-net)
- [Casdoor Sam](#casdoor-sam)
- [Casdoor for Cloud Native](#casdoor-for-cloud-native)
- [Casdoor for Rust](#casdoor-for-rust)
- [Casdoor for Node.js](#casdoor-for-nodejs)
- [Casdoor Hub](#casdoor-hub)
- [Casdoor for PHP](#casdoor-for-php)
- [Casdoor for Python](#casdoor-for-python)
- [Casdoor.js](#casdoorjs)
- [Casdoor for Lua](#casdoor-for-lua)
- [Casdoor for Dart](#casdoor-for-dart)
- [Casdoor for Swift](#casdoor-for-swift)
- [Casdoor Mesh](#casdoor-mesh)



### Casdoor Core Engine (Golang)

#### Description

Support more features and tune the performance in Casdoor core engine. This will first be done in Golang Casdoor. Possibly applied to other language implementations.

#### Expected outcomes

Some issues to work on:

1. Make a Casdoor middleware for go-zero: https://github.com/casdoor/casdoor/issues/957
2. Improve the performance of the new BatchEnforce() API: https://github.com/casdoor/casdoor/issues/710
3. Make a default implementation of WatcherEx: https://github.com/casdoor/casdoor/issues/943
4. Help solve issues for the 1st-party and 3rd-party middlewares

#### Skills required/preferred

1. Golang
2. Other languages that Casdoor is written with

#### Mentors

[Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor

#### Description

Build a UI-first centralized authentication / Single-Sign-On (SSO) platform based on OAuth 2.0 / OIDC. It can:

1. Use OAuth 2.0 + OIDC as the authentication protocols.
2. Support popular 3rd-party identity providers like Google, GitHub, Facebook, etc.
3. Has a web portal to manage users, roles and permissions.
4. Use Casdoor as authorization method.
5. Support user register, login, password reset, 2FA like Email and SMS.

The current progress is: https://door.casdoor.com/. Source code: https://github.com/casdoor/casdoor. We want the student to continue the work.

#### Expected outcomes

Some issues to work on:

1. Support SAML as IdP: https://github.com/casdoor/casdoor/issues/405
2. Support password hashing in LDAP: https://github.com/casdoor/casdoor/issues/499
3. Add Telegram provider: https://github.com/casdoor/casdoor/issues/341
4. Add Casdoor model and policy management: https://github.com/casdoor/casdoor/issues/95
5. Design and develop a more beautiful frontend portal: https://github.com/casdoor/casdoor/issues/69

#### Skills required/preferred

1. Golang (backend)
2. Javascript + React + Ant Design (frontend)
3. Casdoor

#### Mentors

[Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casnode

#### Description

Casnode is a light-weight forum software. It is used by Casdoor community as the official developer forum (https://forum.casdoor.com/). We hope to fix its bugs and add more features like mailing list to replace the traditional open-source community mailing list.

The current progress is: https://github.com/casdoor/casnode

#### Expected outcomes

Some features to add/improve:

1. Further optimized the project UI: https://github.com/casdoor/casnode/issues/400
  Now casnode UI may break on some models, mainly mobile phones, we need to further optimize our project UI to fix it.
2. Anonymous-Post
  Note: we may change whether to enable the node's anonymous function via the admin console.
3. Improve the part of https://forum.casdoor.com/api and https://forum.casdoor.com/swagger/#/ that provides API externally.
4. Implement [notes](https://forum.casdoor.com/notes), so users could create and publish notes: https://github.com/casdoor/casnode/issues/341.
4. Implement [timeline](https://forum.casdoor.com/timeline), so users could post their thoughts and reply to others' thoughts there: https://github.com/casdoor/casnode/issues/341
5. Add RSS feed.
6. Add some metrics, for Prometheus or others.
7. Backup and recovery data from backup files.

Code quality maintenance:

1. Add configurable logs.
  Notes: this may add a completion log system for casnode using [zap](https://github.com/uber-go/zap).
2. More friendly error handling instead of panic.
  Notes: this may be built on a well-established logging system
3. Add some commits for code.
  Notes: This could be finished when you read the code.
4. Improve performance, such as SQL query, cache, etc.

And other [issues](https://github.com/casdoor/casnode/issues) that may arise during the time.

#### Skills required/preferred

1. Golang (backend)
2. Javascript + React (frontend)
3. Casdoor

#### Mentors

[Junjie Zhang](https://github.com/kocoler), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Easy



### Casdoor Dashboard

#### Description

Build a web UI dashboard/admin portal for Casdoor & Casdoor-Server.

#### Expected outcomes

It can:

1. Manage models, adapters, enforcers. The adapter manager should handle different DBs.
2. Model editor with a syntax and semantic validator.
3. Policy editor, it should be able to handle 10,000+ more rules.
4. A test page to make example request to Casdoor and get response, like Postman. So users can test their model and policy.
5. Authentication and authorization for the dashboard itself. Of course authorization will be implemented in Casdoor (we proudly dogfood our own product :))

The current progress is: https://dashboard.casdoor.com . Source code: https://github.com/casdoor/casdoor-dashboard. We want the student to continue the work.

#### Skills required/preferred

1. Golang (backend)
2. Javascript + React + Ant Design (frontend)
3. Casdoor

#### Mentors

[Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Easy



### Casdoor for C/C++

#### Description

<!-- We already have a C/C++ version Casdoor called [Casdoor-CPP](https://github.com/casdoor/casdoor-cpp). It already works on all primary OSs, like Windows, Linux, macOS. Most of Casdoor's functionalities (for example 90%) should work. There are still many bugs and missing features in Casdoor-CPP. Moreover, we also need to make authz middlewares for other C++ projects like [Mosquitto](https://github.com/casdoor/casdoor-cpp/issues/79 ) and adapters for DB. We also have plan to make Casdoor-CPP as a base layer to build the next-generation PyCasdoor and PHP-Casdoor on top of it (see [PyCasdoor on CPP](https://github.com/casdoor/pycasdoor-on-cpp )) for better performance (a lot of Python packages like numpy and tensorflow rely on the underlying C++ code). So Casdoor-CPP needs to provide necessary help if needed for PyCasdoor and PHP-Casdoor developers. -->

[Casdoor-CPP](https://github.com/casdoor/casdoor-cpp) provides various models for advanced authorization solutions in C++. It currently supports all the major OS's including Windows, Linux and macOS.
`casdoor-cpp` has seen a major revamp to make the library as functional as its Golang counterparts.
This project uses [CMake](https://cmake.org) for building, packaging, and installation, and CTest for testing.
Apart from that, `casdoor-cpp` supports python bindings through `pybind11`.

The current progress is: https://github.com/casdoor/casdoor-cpp

#### Expected outcomes

Here is a list of tasks we're looking forward to work on this summer on a priority basis:

- [casdoor-cpp#79](https://github.com/casdoor/casdoor-cpp/issues/79): Developing authz middlewares for other C++ projects like [Mosquitto](https://github.com/eclipse/mosquitto).
- [casdoor-cpp#115](https://github.com/casdoor/casdoor-cpp/issues/115): Developing authz middleware for [Envoy proxy](https://github.com/envoyproxy/envoy).
- [casdoor-cpp#100](https://github.com/casdoor/casdoor-cpp/issues/100): Various features of Casdoor-CPP can be used in [Glewlwyd](https://github.com/babelouest/glewlwyd), a C++ based server. We need to investigate and
try to integrate casdoor-cpp into Glewlwyd.
- [casdoor-cpp#190](https://github.com/casdoor/casdoor-cpp/issues/190): Unit testing and benchmarking for multithreaded workloads is in backlog and needs to be investigated thoroughly.
#### Skills required/preferred

1. C++
2. Golang (only need to read code)
3. CMake
4. Python

#### Mentors

[Yash Pandey](https://github.com/EmperorYP7), Casdoor member,
[Joey Xie](https://github.com/xcaptain), Casdoor member,
[Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Hard



### Casdoor for Java

#### Description

jCasdoor needs to be kept in sync with the features of casdoor-golang at all times. For example, the special syntax of ``in``, the update of the role manager, etc.
At the same time, it is also necessary to maintain and integrate the unique ecology of Java, such as ``casdoor-spring-boot-starter`` and ``Play middleware``, etc.
Performance is also a point of great concern, so ``benchmark`` needs to be done.

#### Expected outcomes

1. More features support
- Reimplement the role manager: [jcasdoor#261](https://github.com/casdoor/jcasdoor/issues/261)
- Sync more features about "in" special grammar from Go-Casdoor: [special-grammer](https://casdoor.org/docs/en/syntax-for-models#special-grammer)
- Make a default implementation of WatcherEx and migrate Watcher to WatcherEx : Default implementation of WatcherEx [casdoor#943](https://github.com/casdoor/casdoor/issues/943)
- Fix the bug about ClassCastException for Strings within grouping fucntions: ClassCastException for Strings within grouping fucntions [jcasdoor#254](https://github.com/casdoor/jcasdoor/issues/254)
2. Continuous maintenance of the surrounding ecology
- Optimize casdoor-spring-boot-starter and other middlewares dependencies. [casdoor-spring-boot-starter](https://github.com/jcasdoor/casdoor-spring-boot-starter)
- Provide more offical adapter/watcher like Golang: [watchers](https://casdoor.org/docs/en/watchers)
- Make a Play Framework middleware: Create a jCasdoor authorization module for Play [jcasdoor#104](https://github.com/casdoor/jcasdoor/issues/104)
- Help solve issues for the 1st-party and 3rd-party middlewares.
3. Benchmark and performance optimization
- Benchmarking jCasdoor and the integrations with main middlewares.
- Find and resolve performance bottlenecks.
- Explore the alternative in large-scale scenarios

#### Skills required/preferred

1. Java
2. Other languages that Casdoor is written with

#### Mentors

[Yang Tang](https://github.com/tangyang9464), Casdoor member, [Zhengjin Fang](https://github.com/fangzhengjin), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for .NET

#### Description

Casdoor.NET v2 will release quickly. The new architecture provides excellent performance and flexible scalability and prepares for the addition of more imaginative and exciting features.

#### Expected outcomes

1. Support more features:
- a. Feature Request: subjectPriority(https://
github.com/casdoor/Casdoor.NET/issues/238)
- b. Support "in" special grammar(https://github.com/casdoor/Casdoor.NET/issues/198)
- c. Validate and compile matcher when loading model(https://github.com/casdoor/Casdoor.NET/issues/228)
- d. Improve the unit test coverage(https://github.com/casdoor/Casdoor.NET/issues/151)
2. Enhance ecosystem:
- a. Support ASP.NET Core and Blazor (Enhance [Casdoor.AspNetCore](https://github.com/casdoor-net/casdoor-aspnetcore))
- b. Provide Offical Redis adaptor/watcher.

#### Requirements

1. .NET/C#
2. ASP.NET Core

#### Mentors

[Sagilio](https://github.com/sagilio), Casdoor member

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for .NET

#### Description

Casdoor is a UI-first centralized authentication / Single-Sign-On (SSO) platform based on OAuth 2.0 / OIDC. We hope to provide a comprehensive and powerful SDK to make .NET application integrate with it easily.

#### Expected outcomes

1. Implement SDK:
- a. Implement Casdoor.Client to call Casdoor APIs easily.
- b. Implement Casdoor.AspNetCore to integrate ASP.NET Core with Casdoor.
- c. Implement Casdoor.Native to integrate WPF or Maui with Casdoor
2. Implement Samples:
- a. Provide ASP.NET Core Web API, MVC and Blazor samples with the SDK.
- b. Provide WPF or Maui smaples with the SDK.

#### Requirements

1. .NET/C#
2. ASP.NET Core
3. WPF or Maui

#### Mentors

[Sagilio](https://github.com/sagilio), Casdoor member

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor Sam

#### Description

An authorization service based on OAuth 2.x and support centralized authentication / Single-Sign-On (SSO) integration. It can:

#### Expected outcomes

1. Use [Casdoor.NET](https://github.com/casdoor/Casdoor.NET) and [Casdoor.AspNetCore](https://github.com/casdoor-net/casdoor-aspnetcore) to authorizate.
2. Provide Web APIs to manage users, roles and permissions.
3. Support integrate OIDC authentication provider ([Identity Server 4](https://github.com/IdentityServer/IdentityServer4)) and [ASP.NET Identity](http://docs.identityserver.io/en/latest/quickstarts/6_aspnet_identity.html) to manage user and sgin in/out.
4. Support be integrated to [Dapr](https://github.com/dapr/dapr) or [Steeltoe](https://github.com/SteeltoeOSS/Steeltoe) as authentication/authorization provider.

The current progress is: https://github.com/casdoor-net/casdoor-sam. We want the student to continue the work.

#### Requirements

1. .NET/C#
2. [Casdoor.NET](https://github.com/casdoor/Casdoor.NET) and [Casdoor.AspNetCore](https://github.com/casdoor-net/casdoor-aspnetcore)
3. [Dapr](https://github.com/dapr/dapr) or [Steeltoe](https://github.com/SteeltoeOSS/Steeltoe)

#### Mentors

[Sagilio](https://github.com/sagilio), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for Cloud Native

#### Description

Currently, Casdoor has limited adaptability in the cloud-native field. We hope to use kubebuilder 3.x to refact the [k8s-authz](https://github.com/casdoor/k8s-authz) and provide CRD based model and policy management. Enhance model parse to compatible with k8s better.

#### Expected outcomes

1. Refact k8s-authz
- a. Porvide predefined `r` or `p` tokens and custom function for k8s.
- b. Provide CRD based model and policy management.
- c. Provide Client and helm integration.
- d. Make kubesphere-athz compatible with the new k8s-authz.
- e. Improve test coverage for the new [k8s-authz](https://github.com/casdoor/k8s-authz) and [envoy-authz](https://github.com/casdoor/envoy-authz).

2. Enhance ecosystem:
- a. Implement Casdoor middleware for [Dapr](https://docs.dapr.io/reference/components-reference/supported-middleware/)
- b. Explore more usage scenarios on Cloud Native.

#### Requirements

1. Golang
2. K8s ([kubebuilder](https://book.kubebuilder.io/)) and Cloud Native
3. Service Mesh and [Dapr](https://dapr.io/)

#### Mentors

[Sagilio](https://github.com/sagilio), Casdoor member, [Ashish](https://github.com/ashish493), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Hard



### Casdoor for Rust

#### Description

With Casdoor community's effort, the Rust version of Casdoor is now mature and ready for production. [Casdoor-RS](https://github.com/casdoor/casdoor-rs) can provide access control with blazing fast speed.

#### Expected outcomes

There are something need to be implemented，from easy to hard:

1. Embrace Rust 2021 edition [Easy]

- Complete the migration from edition 2018 to edition 2021.
- Clean up stale and meaningless dependencies and make clippy happy.

**Note** This work will help you get familiar with the Rust toolchain and the existing work of Casdoor-RS, so please complete it for at least two repos.

2. Continuous maintenance of the surrounding ecology [Medium]

- Implement a middleware for [Poem](https://github.com/poem-web/poem) with examples.
- An article introducing how to use casdoor-rs with poem.
- Participate in the maintenance of at least one other repo, such as [sqlx-adapter](https://github.com/casdoor-rs/sqlx-adapter) or [casdoor-grpc](https://github.com/casdoor-rs/casdoor-grpc/).

**Note** This work will help you understand the mechanics of casdoor's operation. In addition, we hope you can present your works, which will become an important milestone for you in the casdoor community.

3. Explore casdoor-rs in real-world/distributed applications [Hard]

- You can choose to:
  - Implement a real-world application with casdoor-rs, Or
  - Implementing [openraft](https://github.com/datafuselabs/openraft)-based distributed casdoor clusters/plugins.
- An article that describes your current work.

**Note** Go beyond the existing casdoor-rs projects, this is a job that is completely led by you. [casdoor-grpc](https://github.com/casdoor-rs/casdoor-grpc/) and [casdoor-raft](https://github.com/casdoor-rs/casdoor-raft/) are the results of some previous explorations.

#### Skills required/preferred

1. Rust
2. Other languages that Casdoor is written with

#### Mentors

[Chojan Shang](https://github.com/PsiACE), Casdoor member, [Yisheng Chai](https://github.com/hackerchai), Casdoor member, [Cheng JIANG](https://github.com/GopherJ), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Hard



### Casdoor for Node.js

#### Description

Improving the user experience of Node-Casdoor will be our focus.

#### Expected outcomes

Some issues to work on:

- Sync GetImplicitResourcesForUser method(https://github.com/casdoor/node-casdoor/issues/344)

- Sync UpdateGroupingPolicy and UpdateNamedGroupingPolicy method(https://github.com/casdoor/node-casdoor/issues/324)

- Improve built-in method of matcher(https://github.com/casdoor/node-casdoor/issues/332)

- Scaling Access Control Lists for multi-million users(https://github.com/casdoor/node-casdoor/issues/147)

- Sequelize v6 compatibility: addPolicies & removePolicies problem(https://github.com/casdoor/node-casdoor/issues/207)

#### Skills required/preferred

1. JavaScript (Node.js/TypeScript)
2. Other languages that Casdoor is written with

#### Mentors

[Zixuan Liu](https://github.com/nodece), Casdoor member

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor Hub

Casdoor Hub is similar to [Docker Hub](https://hub.docker.com/search?q=&type=edition&offering=community) website, which is mainly used to share and discuss the model and policy of Casdoor.

#### Expected outcomes

We need to implement the following features:

1. Support anyone to share the model and policy of Casdoor. Sharers must describe the scenario that this model applies, and mark the classification, like so: Frontend, Backend, Cloud, Message System, and so on. Users can discuss shared content.

2. Integrate the [Casdoor-Online-Editor](https://casdoor.org/en/editor) is used to test or debug the model and policy shared by users.

#### Skills required/preferred

1. Golang (Backend)
2. React (Frontend)
3. Casdoor

#### Mentors

[Zixuan Liu](https://github.com/nodece), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for PHP

#### Description

[PHP-Casdoor](https://github.com/php-casdoor/php-casdoor) An authorization library that supports access control models like ACL, RBAC, ABAC in PHP .

#### Expected outcomes

1. Add `AddPermissionsForUser` API.
2. Add cache for `g` function, refer to: https://github.com/casdoor/casdoor/blob/master/util/builtin_operators.go#L333.
3. Integrate laravel's [Gates](https://laravel.com/docs/9.x/authorization#gates) in [Laravel-Authz](https://github.com/php-casdoor/laravel-authz).
4. Implementation of [WatcherEx](https://casdoor.org/docs/en/watchers#watcherex), basic Watcher: [Swoole Redis watcher](https://github.com/php-casdoor/swoole-redis-watcher) [Workerman Redis watcher](https://github.com/php-casdoor/workerman-redis-watcher).
5. Implement [propel-adapter](https://github.com/php-casdoor/propel-adapter), [Propel](http://propelorm.org/) is a highly customizable and blazing fast ORM library for PHP.
6. Consistent with the functionality of [Casdoor Core Engine (Golang)](https://github.com/casdoor/casdoor).
7. Bug fixes in [issues](https://github.com/php-casdoor/php-casdoor/issues), improve some [extensions](https://github.com/php-casdoor).

#### Skills required/preferred

1. PHP
2. Casdoor

#### Mentors

[Jon Lee](https://github.com/leeqvip), Casdoor member

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for Python

#### Description

1. At present, compared to Casdoor for Golang, `Pycasdoor` is not very perfect, especially the lack of RBAC API, so we hope that `Pycasdoor` can fully implement the function of Casdoor (Go).
2. `PyCasdoor`'s adaptation to various frameworks, such as `Django`, `Tornado`, etc.

Pycasdoor organization: https://github.com/pycasdoor

#### Expected outcomes

1. Implement [redis-adapter](https://github.com/pycasdoor/redis-watcher).
2. Implement [etcd-adapter](https://github.com/pycasdoor/etcd-watcher).
3. Improve performance for `enforce()`.
4. Complete implementation of PyCasdoor-on-CPP.
5. Reimplement the implementation of Pycasdoor in `Django`, introduce Django's `Middleware`, `Caching`, `Logging`, and integrate the Django authentication system, and existing plugins: [django-casdoor](https://github.com/pycasdoor/django-casdoor) [django-orm-adapter](https://github.com/pycasdoor/django-orm-adapter).

Some issues to work on: https://github.com/casdoor/pycasdoor/issues

#### Skills required/preferred

1. Python
2. Other languages that Casdoor is written with

#### Mentors

[Jon Lee](https://github.com/leeqvip), Casdoor member

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor.js

#### Description

Quite a lot of users want to use Casdoor to control web frontend UI elements, like:

1. Some tabs are only visible to admin users.
2. Some buttons should be grayed-out for users with no permission to click them.
3. A list can only show filtered items based on a user's permission rights.

Over time we have made node-casdoor a cross-platform Javascript permission control library and have called the new library casdoor.js. The next step is to refactor node-casdoor to a casdoor.js-based wrapper. Another possible idea is create a `browser-casdoor` for front-end developers with front-end friendly api.

The current progress is: https://github.com/casdoor/casdoor.js

Currently, we still lack the middlewares for Angular, React and Vue. These new JS frameworks are very popular and making middlewares for them will boost our usage from their population.

#### Expected outcomes

1. Sync progress with node-casdoor
2. Update vue-authz and react-authz to new casdoor.js.
3. Refactor node-casdoor to casdoor.js wrapper.

#### Skills required/preferred

1. Typescript
2. Node-Casdoor
3. Vue or React development experience
3. At least one backend language like Golang

#### Mentors

[Xinyu Zhou](https://github.com/Zxilly), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Hard



### Casdoor for Lua

#### Description

Port Golang Casdoor into Lua. We call it `lua-casdoor`. It should work on the Nginx + OpenResty stack. Most of Casdoor's functionalities (for example 90%) should work.

Nginx is now the most popular HTTP server in the world. OpenResty is a web platform based on Nginx which can run Lua scripts using its LuaJIT engine. Nginx + OpenResty are usually used in edge computing and authorization is a real need for its scenario. Lua-Casdoor will help Nginx and OpenResty users on checking permissions of the coming HTTP request.

The current progress is: https://github.com/casdoor/lua-casdoor

#### Expected outcomes

1. Implementation of `Watcher`, `Watcher` ensures policy consistency in multiple Casdoor instances.
2. Add cache for `g` function, refer to: https://github.com/casdoor/casdoor/blob/master/util/builtin_operators.go#L333.
3. Add `AddPermissionsForUser` API.
4. Add LoadPolicyArray() to load policy from array
5. Improve performance for `enforce()`.
6. Implement the built-in function `keyMatch5`.
7. Fixes and refinements to lua-casdoor's [extensions](https://github.com/casdoor-lua).

#### Skills required/preferred

1. Nginx
2. OpenResty
1. Lua
2. Golang (only need to read code)

#### Mentors

[Jon Lee](https://github.com/leeqvip), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium



### Casdoor for Dart

#### Description

Port Casdoor to Dart, little progress has been made in the project so it's excellent for jumping in early.

The current progress is: https://github.com/casdoor/dart-casdoor

#### Expected outcomes

You will be responsible for the design and making of the Dart port with the help of the mentor, most of Casdoor's functionalities should work.

#### Skills required/preferred

1. Dart
2. Other languages that Casdoor is written with.

#### Mentors

[Tomás Arias](https://github.com/KNawm), Casdoor member

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium

### Casdoor for Swift

#### Description

We already have a Swift version Casdoor called [SwiftCasdoor](https://github.com/casdoor/SwiftCasdoor.git). It already works on all primary OSs, like Windows, Linux, macOS,iOS,tvOS,watchOS. Most of Casdoor's functionalities (for example 90%) should work.

The current progress is: https://github.com/casdoor/SwiftCasdoor

#### Expected outcomes

There are still many bugs and missing features in SwiftCasdoor. Moreover, we also need to make authz middlewares for any  Swift projects:

1. Server-Side like Vapor and adapters for DB.
2. A frontend developer friendly API for UI frameworks like UIKit,SwiftUI.

#### Skills required/preferred

1. Swift
2. Golang (only need to read code)
3. ios UIkit SwiftUI

#### Mentors

[Xiaobei](https://github.com/xiaobeiswift), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

175 hour

#### Rating (Easy, Medium or Hard)

Medium

### Casdoor Mesh

#### Description

Last summer, we started a new project called Casdoor-Mesh which allows us to deploy the Casdoor to many nodes using the raft consensus algorithm to handle rapidly increasing data, which raises the throughout of read-only transactions.

The current progress is: https://github.com/casdoor/casdoor-mesh


#### Expected outcomes

However, there are still many works that need to be done.

1. The bottleneck of memory data structure
- Reconstruction the memory data model
  - We are going to use the buffer pool manager handling very large data that over then RAM
2. Avoiding full-table scanning
- Indexes
  - Create indexes for all policies
  - Use Indexes to avoid full-table scanning
- Basic query optimization
3. Transaction Implementations

#### Skills required/preferred

1. Golang
2. At least you need to be familiar with the basic concepts of the query optimization, indexing (hash index, B+ tree index), multi-version concurrency control.
2. (preferred) Had taken database lectures (Such as CMU 15-445 etc.)



#### Mentors

[WenyXu](https://github.com/WenyXu), Casdoor member, [Eric](https://github.com/hsluoyz), Casdoor founder

#### Expected size of project (175 hour or 350 hour)

350 hour

#### Rating (Easy, Medium or Hard)

Hard
