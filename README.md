# My Quarkus Project

This is a simple downstream guide to help you get started with building your first Quarkus project. This guide assumes you have no experience in Maven, Docker, GraalVM or Quarkus. You need at least basic understanding of Java, Git

Most of the steps are forked from [here.](https://quarkus.io/get-started/)


## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- Java Development Kit (JDK) (I used [latest Eclipse Temurin 21](https://github.com/adoptium/temurin21-binaries/releases/tag/jdk-21.0.2%2B13))
- Preferred IDE (I used [VSCode](https://code.visualstudio.com/))
    - [GitHub Copilot](https://github.com/features/copilot) or equivalent (optional but recommended. Steps are fairly straightforward, but if you get stuck you can always ask for help)
    - Preferred CLI ([Git BASH](https://gitforwindows.org/) recommended, makes copy-pasting unix commands straightforward)
- [SDKMAN](https://sdkman.io/) (optional but HIGHLY recommended, makes installing packages straightforward)
- [Apache Maven 3.9.6](https://maven.apache.org/) (easiest to install with SDKMAN)

## Getting Started

### 1. Install SDKMAN if you don't have it yet

Paste this code to your bash:
```python
curl -s "https://get.sdkman.io" | bash
```
After that, open new bash.

### 2. Install Quarkus & Maven

Paste this code to your bash to install Quarkus & Maven:
```
sdk install quarkus
sdk install maven
```
And this code to create your first Quarkus project:
```
quarkus create && cd code-with-quarkus
```

### 3. Run the project

Paste this code to your bash to start Quarkus
```
quarkus dev
```
Your Quarkus app is now running at http://localhost:8080

### 4. All set! 

Next step for me was to build a native executable, but you can skip this part if you want.

## [Building a native executable](https://quarkus.io/guides/building-native-image)

Additional requirements:
- Container runtime (Docker)
- GraalVM (Mandrel recommended)

### 1. Download, install & learn [Docker](https://www.docker.com/)
If you are new to Docker, no worries! As Docker states in their tutorial: The best way to learn about containers is to first see it in action. I am using [Docker desktop](https://www.docker.com/products/docker-desktop/). Fire up Docker Desktop, and complete the following tutorials: "What is a container?", "How do I run a container?"

### 2. [Download](https://github.com/graalvm/mandrel/releases), install & [configure](https://quarkus.io/guides/building-native-image#configuring-graalvm) GraalVM (Mandrel)


