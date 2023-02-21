# Infrastructure as Code (IaC)

This section describes the common practice of **Infrastructure as Code (IaC)**,
a method that enables developers to add reliability to their engineering
strategy.

## What is infrastructure?

First, we'll define **infrastructure** to later understand why this common
practice is important. When we talk about **infrastructure**, we mean
**information technology infrastructure** or **IT infrastructure**.

**IT infrastructure** comes in two flavors:

- **Traditional infrastructure**
  - Comprised of the usual hardware and software components, usually install
  on-premises for company-only or private use, requires some manual setup.
- **Cloud infrastructure**
  - Someone elses computer, usually provided through services like Amazon Web
  Services (AWS), Google Cloud Platform (GCP), or Microsoft's Azure platform.
  - Relies on virtualization to abstract away the underlying resource pool of
  hardware provided by these platforms. This enables scalability and reliability
  for customers, while also allowing them to use only the resources they need
  to host a service.
  - Public cloud instances hosted on these platforms are always accessible as
  long as the client has an internet connection.

## How is code involved in infrastructure?

The infrastructure that software runs on is just as important as the software
itself. It needs to be reliable, secure, and scalable - because of this we aim
to apply software engineering concepts to the implementation of our
infrastructure. Just like application development, we use all of our software
engineering tricks - version control, testing, etc.

Programming languages are involved in the implementation of infrastructure
because it allows us to describe a desired state. The infrastructure has a
current state and, using code, we can provide the computer with declarative or
imperative statements to bring convergence to our desired state - whatever that
may be. [[2]](#references)

## What's the difference between the push and pull methods in IaC?

**Push** and **pull** describe methods in which **IaC** frameworks manage and
configure resources or servers. A description of these two methods follows:

- **Push** - managing servers for frameworks using this method reach out to
managed servers, providing updates to configurations or executing actions on the
managed servers to bring them to convergence.
- **Pull** - managed servers for frameworks using this methods periodically
reach out to the managing server, requesting updates to configuration and
executing the necessary actions to reach convergence of state described by the
managing server.

**Ansible** is a good example of a **push** **IaC** framework. **Chef** is a
good example of a **pull** **IaC** framework.

## What are some common programming languages used in IaC?



## References

1. [https://web.archive.org/web/20221116020116/https://www.ibm.com/topics/infrastructure](https://web.archive.org/web/20221116020116/https://www.ibm.com/topics/infrastructure)
2. [https://web.archive.org/web/20230113162005/https://www.infoq.com/presentations/history-infra-as-code/](https://web.archive.org/web/20230113162005/https://www.infoq.com/presentations/history-infra-as-code/)