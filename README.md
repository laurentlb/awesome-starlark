# Awesome Starlark
*A list of awesome things related to the Starlark language.*

Starlark is a simple, Python-like language designed to be embedded in another application to provide configuration or scripting abilities.

## Getting Started

*   [The language specification](https://github.com/bazelbuild/starlark/blob/master/spec.md)

*   There are 3 known implementations of the Starlark language:
    -   [starlark-go](https://github.com/google/starlark-go/) - an implementation in Go.
    -   [starlark-rust](https://github.com/facebookexperimental/starlark-rust) - an implementation in Rust.
    -   [starlark/java](https://github.com/bazelbuild/bazel/tree/master/src/main/java/net/starlark/java) - an implementation in Java
      built for Bazel, that may not be suitable for use in other applications.

*   Bindings:

    -  [HarikrishnanBalagopal/starlark-webasm](https://www.npmjs.com/package/starlark-webasm) - a webassembly package for starlark-go.
    -  [python-starlark-go](https://github.com/caketop/python-starlark-go) - Python bindings for Starlark in Go.
    -  [starlark-pyo3](https://github.com/inducer/starlark-pyo3) - Python bindings for Starlark in Rust.


## Tutorials

* [A practical introduction to the Starlark language](https://laurent.le-brun.eu/blog/a-practical-introduction-to-the-starlark-language) by Laurent Le Brun, 2024.
* [An Overview of the Starlark language](https://laurent.le-brun.eu/blog/an-overview-of-starlark) by Laurent Le Brun, 2024.
* [Embedding Starlark (Part 1) — Configure Go Programs with Starlark Scripts](https://medium.com/@vladimirvivien/embedding-starlark-part-1-configure-go-programs-with-starlark-scripts-5abde31b8265) by Vladimir Vivien, 2023.
* [GothamGo 2017: A Go implementation of the Skylark Configuration Language](https://www.youtube.com/watch?v=9P_YKVhncWI) by Alan Donovan, 2017.

## Tools

* [Buildifier](https://github.com/bazelbuild/buildtools) - The official code formatter &
  linter. It can also apply automated fixes (e.g. remove unused loads).
* [Moonlark](https://github.com/obazl/moonlark) - Starlark parser in C with Lua
  bindings.
  [py2star](https://github.com/mahmoudimus/py2star) - a basic converter from Python to Starlark.
* [Stardoc](https://skydoc.bazel.build/) - A documentation generator originally designed for Bazel.
* [Starlark Online Playground](https://laurent.le-brun.eu/starlark/) -
    A web playground for Starlark.
* [Starlark Playground](https://github.com/qri-io/starpg) - Starlark Playground
  is a web-based starlark editor. It uses the golang implementation of starlark
  running on a server to present a monaco editor set to python syntax.


## Libraries and extensions

Libraries that can be useful for the applications that embed Starlark:

*  [Skycfg](https://github.com/stripe/skycfg) - a library for Starlark to
   generate Protocol Buffer messages.
*  [starlark-go-nethttp](https://github.com/pcj/starlark-go-nethttp) - a wrapper
   around a minimal subset of `net/http package` for use within starlark-go.
*  [starlark-re](https://github.com/magnetde/starlark-re) - an implementation
   of Python's `re` module for Starlark in Go.
*  [Starlet](https://github.com/1set/starlet) - a Go wrapper for the [Starlark in Go](https://github.com/google/starlark-go) that
   simplifies script execution, provides data conversion, and offers useful Starlark libraries and extensions.
*  [Starlib](https://github.com/qri-io/starlib) - Qri's standard library for
   Starlark in Go that includes packages for regular expressions, reading XLSX
   documents, parsing ZIP archive, and other functionality.
*  [Starlight](https://github.com/starlight-go/starlight) - a wrapper around the
   Starlark interpreter in Go.
*  [starstruct](https://github.com/mna/starstruct) - a library for converting
   between Starlark in Go's `StringDict` type and Go structs.
*  [Startype](https://github.com/vladimirvivien/startype) - a library that
   implements two-way conversion between Starlark in Go API types and regular
   Go types.

## IDEs

Some IDEs have a [plugin for Bazel](https://bazel.build/install/ide).
Otherwise, consider using a Python mode.

*  [Starpls](https://github.com/withered-magic/starpls) - a language server
   for Starlark.

## Community

* [/r/starlark/](https://www.reddit.com/r/starlark/) - a subreddit for Starlark.

## Users

List of projects that use Starlark.

*  [AsCode](https://github.com/mcuadros/ascode) - a tool to define infrastructure
   as code using the Starlark language on top of Terraform.
*  [AutoKitteh](https://github.com/autokitteh/autokitteh) - a developer platform
   for workflow automation and orchestration. It is a code-based alternative to
   no/low-code platforms. Workflows can be defined
   [using Starlark](https://docs.autokitteh.com/glossary/starlark).
*  [Bazel](https://github.com/bazelbuild/bazel) - a fast, scalable,
   multi-language and extensible build system. Starlark has been designed for
   Bazel.
*  [Buck2](https://buck2.build/) - a build system from Meta, using
   Starlark in a similar way as Bazel.
*  [bramble](https://github.com/maxmcd/bramble) - a purely functional build system
   and package manager, using Starlark as the configuration language.
*  [Copybara](https://github.com/google/copybara) - a tool for transforming and
   moving code between repositories. It embeds Starlark to configure the workflow.
*  [clace](https://github.com/claceio/clace) - web app development and deployment
   platform for internal tools. It allows easy and secure hosting of multiple web
   apps, in any language/framework, on a single machine.
*  [Delve](https://github.com/go-delve/delve) - a debugger for the Go
   programming language, aiming to provide a simple, full featured debugging
   tool for Go. [Delve uses Starlark](https://github.com/go-delve/delve/blob/master/Documentation/cli/starlark.md)
   as a a scripting language.
*  [Drone](https://drone.io) - a self-service Continuous Delivery platform. It
   supports [Starlark scripting](https://docs.drone.io/starlark/overview/) as an
   alternate to yaml configurations.
*  [envd](https://github.com/tensorchord/envd) - a CLI to build the docker images
   for machine learning development and production environments.
*  [FizzBee](https://fizzbee.io) - a system design language for verifying
   distributed systems in cloud, micro-services, and event-driven applications.
   It uses Starlark to offer an intuitive, Python-like syntax, making it
   accessible for everyday software developers. 
*  [Isopod](https://github.com/cruise-automation/isopod) - created by Cruise
   Automation is a DSL framework for Kubernetes configuration. It renders
   Kubernetes objects as Protocol Buffers.
* [Kurtosis](https://github.com/kurtosis-tech/kurtosis) - a developer tool
   for engineers to package and run environments of containerized services for
   development, testing, and production. Starlark is used as the DSL for
   defining those environments in a deterministic, portable, and readable way,
   without compromising usability for complex cases.
*  [lucicfg](https://chromium.googlesource.com/infra/luci/luci-go/+/refs/heads/master/lucicfg/doc/README.md) -
   a tool for generating low-level configuration files from Starlark, used by Chromium CI.
*  [Pixlet](https://github.com/tidbyt/pixlet) - a runtime and UX toolkit for generating animations for small LED displays, such as [Tidbyt](https://tidbyt.com/). Starlark is used to write applets whose outputs are WebP animations.
*  [gnetlark](https://github.com/xyproto/gnetlark) - a web server with handlers
   written in Starlark.
*  [qri](http://qri.io/) is versioned, scriptable, exportable,
   collaborative datasets. It uses Starlark to [describe transformations](https://qri.io/docs/reference/starlark_syntax/).
*  [realm](https://github.com/spellshift/realm) - an Adversary Emulation Framework
   with a focus on scalability, reliability, and automation. It is highly performant and is
   designed for engagements of any size. See
   [how they use Starlark](https://docs.realm.pub/user-guide/eldritch).
*  [recur](https://github.com/dbohdan/recur) - a command-line tool that
   retries a command with exponential backoff plus jitter to mitigate the
   thundering herd problem. The success condition is written as a Starlark
   expression.
*  [Tilt](https://tilt.dev/) - manages local development instances for teams that
   deploy to Kubernetes. [Tilt files](https://docs.tilt.dev/tiltfile_concepts.html)
   are written in Starlark.
*  [Vela](https://go-vela.github.io/docs/) - a continuous integration and delivery platform.
   It supports [Starlark scripting](https://go-vela.github.io/docs/templates/tutorials/starlark/)
   as an alternative to YAML.
*  [VGS](https://www.verygoodsecurity.com/) - a data security platform that
   simplifies secure data storage, compliance, and sharing through tokenization
   and a vault-like infrastructure. Read their
   [announcement](https://www.verygoodsecurity.com/blog/posts/meet-starlarky)
   and [their documentation](https://www.verygoodsecurity.com/docs/vault/developer-tools/larky)
   to see how they use Starlark to let their customer process sensitive data in
   a secure way.
*  [ytt](https://get-ytt.io/) - a templating tool, built on top of Starlark,
   that understands YAML structure allowing you to focus on your data instead of
   how to properly escape it. Read also [IBM's blog post](
   https://developer.ibm.com/blogs/yaml-templating-tool-to-simplify-complex-configuration-management/)
   about it.
