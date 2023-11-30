# 📦 DevEnv Package Manager 🛠️
---

An optimized binary and dependency package manager for a lightweight local development environment. DPM is console based and is a part of [DevEnv](https://github.com/haikalrafifas/devenv) convention.

# How it Works
---

DPM carefully choosing the most popular, yet stable dependency and then store it in the DPM registry.
Not only that, DPM developer also optimizes it so that it will be lightweight even for development purpose.

In the end, DPM users can install them locally without much hassle, plus the reduced bloat.

# Examples
---

### Case 1

Suppose you are a web developer and wanted to make a simple REST API using Express and MySQL.
The problem is that you are on a mid-to-low end spec'd laptop with limited disk space.
Instead of downloading the dependencies (NodeJS and MySQL) individually resulting in higher disk usage,
you can instead use DPM, which will download the stable and optimized version of them.
Users are not required to do any complicated installations, just download and use. Take a look at the disk usage table below, comparing individual and DPM installation:

|Dependency|Individual|DPM|
|-|-|-|
|NodeJS 16|80 MB|80 MB|
|MySQL CE 8 (zip unpacked)|990 MB|326 MB
|-|-|-|
|**TOTAL**|**1070 MB**|**406 MB**|

Not only you can save disk space, but possibly computing resource since the dependency uses less memory to run.

## Case 2

Continuation of Case 1, now you need a tool to actually interact with the database scheme. The most popular one is PHPMyAdmin which usually comes bundled by XAMPP. But, if not counting MySQL in, it requires an Apache web server, and PHP to be able to work, which will result in larger disk usage. DPM offers an alternative of that, let's say, Adminer. It is also a PHP-based database management tool, but since it does not require any web server, it is more lightweight while still being full-featured. Again, let's take a look at the comparison below:

|Install Method|Dependency|Approximate Size|
|-|-|-|
|Individual|XAMPP|**300 MB**|
|DPM|Adminer|**10 MB**|

# Notices
---

1. DPM is a part of [DevEnv](https://github.com/haikalrafifas/devenv) convention, which is why the locally installed dependencies only
works on "DevEnv" environment and not system-wide.
2. DPM might be lack in up-to-date dependencies, as its main goal is to deliver the most optimized and stable
   dependencies for local development environment.
3. As of the latest update, DPM only focused on Windows OS only.

# Contributing
---

Be the part of our community by frequently manage and optimize the DPM registries.
