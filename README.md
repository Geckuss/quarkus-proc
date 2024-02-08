# My Quarkus Project

This is a simple guide to help you get started with building your first Quarkus project.

https://quarkus.io/get-started/

## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- Java Development Kit (JDK) 11 or later
- Apache Maven
- Git (Bash)
- SDKMAN

## Getting Started

1. Install SDKMAN if you don't have it yet

Paste this code to your bash:
```python
curl -s "https://get.sdkman.io" | bash
```
After that, open new bash.

2. Install Quarkus & Maven

Paste this code to your bash to install quarkus & Maven:
```
sdk install quarkus
sdk install maven
```
And this code to create your first quarkus project:
```
quarkus create && cd code-with-quarkus
```