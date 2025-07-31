# virtulisation

# What is virtulisation?

*The dividing of physical computing resources into a series of virtual machines and operating systems*

It is used to create a ‘virtual’ version of an underlying service.

With the help of virtulisation, multiple operating systems and applications can run on a single machine at the same time, increasing utilisation and flexibility of hardware

It’s one of the main cost effective hardware reducing and energy saving techniques used by cloud providers. Virtualisation allows sharing of a single physical interface, resource or application among multiple customers and organisations at one time

**Host machine:** The machine on which the virtual machine is going to be built on

**Guest machine:** Another name for a virtual machine

## Increased security

The ability to control the execution of a guests programs in a completely transparent manner.

Allows for delivering a secure, controlled execution environment

All operations of the guest programs are generally performed against the virtual machine which translates and applies them the the host programs

A virtual machine manager can control and filter the activity of the guest programs, preventing some harmful operations from being performed.

Resources exposed by the host can be hidden or protected from the guest.

## Managed execution

![image.png](Virtualisation%2011953012912780fc8889e0c85455b491/image.png)

## Sharing

Virtualisation allows the creation of a separate computing environments within the same host

This basic feature is used to reduce the number of active services and limit power consumption

## Aggregation

Physical resources can be shared among several guests, but also virtualisation allows for aggregation, which is the opposite process.

A group of separate hosts can be tied together and represented to guests as a single virtual host

It is implemented with cluster management software which harnesses the physical resources of a group of machines and represents them as a single resource

## Emulation

Guest programs are executed within an environment that is controlled by the virtualisation layer which ultimately is a program

Also a completely different environment with respect to the host can be emulated, thus allowing the execution of guest programs, requiring specific characteristics that are not present in the typical host 

(such as emulating old Macintoshes, which used a non standard processor than what the standard is now)

## Isolation

Virtualisation allows providing guests, weather they are OS’s, applications, or other entities, within a completely separate environment where they are executed.

The guest program performs its activity by interacting with an abstraction layer, providing access to underlying resources.

The VM can filter the activity of the guest and prevents harmful operations against the host

Besides these characteristics, VM’s also enable performance tuning, allowing fine tuning of properties of the resources exposed through the virtual environment.

This capability provides a means to effectively implement a QoS infrastructure

## Portability

In the case of hardware virtualisation, the guest is packaged into a virtual image that in most cases can be safely moved and executed on top of different virtual machines.

In the case of programming level virtualisation (implemented by the JVM or .NET runtime(s)) the binary code representing application components can run without any recompilation of the corresponding virtual machine

## Advantages

Virtual environments can help grow small to medium size businesses, by providing flexibility and efficient resource utilisation

Rather than replacing backup appliances as they grow, a virtual environment can give them quick and easy scalability should the business experience rapid growth

Reduced costs as there is less infrastructure to purchase and manage, while also saving on electricity costs

- Capital expenditure savings - Allows companies to reduce their IT costs by requiring less hardware server
- Operational savings - Once servers are virtualised IT staff can greatly reduce administration of manual tine consuming processes by automating processes
- Data centre and energy efficiency savings - as companies reduce hardware size and server footprint, energy consumption is reduced, and so are costs

Quick step and installation reduces time commitment

Makes backup and recovery more efficient and reliable

## Disadvantages

Costs - Upfront costs are often expensive when transferring from a legacy system, typically upwards of £/$10,000 for servers and software licenses. However s virtualisation technology improves and becomes more commonplace costs will reduce

Can pose challenges as a virtual environment is something else you need to maintain

Not all servers and applications are virtualisation friendly. Mainly due to the creator not supporting virtualisation

Server sprawl can be an unintended consequence. Once administrators see how easy it is to add new servers, they add more, creating unnecessary servers, wasting time and money