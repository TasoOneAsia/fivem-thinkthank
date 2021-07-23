## Core Resource

### Functionality

* Provide general dev utility functions that can improve dev experience. (Concentrated logging, native-wrappers,
  and bridging functionality towards all other runtimes).
* Be as compatible with as many paradigms, development workflows, and scripting runtimes as possible.
* Be responsible for general player management upon connect/disconnect instantiating memory data structures that 
  will be utilized by other resources calling into `core`.
* Heavy context based functionality (database, data structure manipulation, caching) will be concentrated primarily on
  on the server side utilizing V8 as the ScRT.
* More..?

**Why V8?**

Node and specifically TypeScript, offers a good mix between the dynamic fast workflow of Lua and the
rigid and type safe environment of `dotnet`. As V8 is multi-paradigm capable, imperative design and OOP design
can be combined easily without it feeling out of place.

This core resource will mostly contain context dependent and non-pure with Node on the server side. Although it will
still provide client utilities and ScRT bridges independent of side effects.

Node and subsequently NPM offers a massive package environment that can be used to scaffold easily.

*Thoughts?*




*We want to keep this core resource as light as possible, instead a more favorable pattern 
would be moving new functionality into resources that call Core*
  
