**Mockito**

Mockito is an open source testing framework for Java released under the MIT License. 
The framework allows the creation of mock objects in automated unit tests. Other 
Java mocking frameworks include PowerMock and EasyMock.

**SUT** 

System under test (SUT) refers to a system that is being tested for correct operation. 

**Mocking**

Mocking is a replica or imitation of something. Mocking is used in unit testing. Mock objects are 
simulated objects that mimic the behavior of real objects in controlled ways
A tested object may have dependencies on other complex objects. To isolate the behavior of 
the object we want to test we replace the other objects by mocks that simulate the behavior 
of the real objects. So in simple words, mocking is creating objects that simulate the behavior 
of real objects.


**Stub**

A stub method is a method that just returns a simple but valid 
(though not necessarily correct) result.

Stubs are made when building the infrastructure and we do not 
want to spend time on every method needed right now. Instead we create stubs 
so everything compiles and our IDE's auto-complete knows about the methods 
we plan to use.

Stubs are using in mocking as well. We supply stub methods instead of the normal 
dependency through dependency injection which return fixed results and then ensure 
that the code does the right thing with them. 
This isolates testing to the code we are trying to test and means we do not need 
to spin up a database just to run those tests.