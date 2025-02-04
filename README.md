Multiple Classes - Brief

Model a Bus which can pick up and drop off Passengers.

Create a Bus class.
 - The Bus should have a route number and a destination.
 - It should also have a drive method that returns a string.

Create a Person class.
 - The Person class should have attributes of a name and age.


Part 2
 - Give the Bus class a new property, 'passengers'. This should be a list, which starts off empty.
 - Add a method to the Bus class which returns how many passengers are on the bus.
 - Add a method to the Bus class which takes in a Person and appends it to the list of passengers. The method could look something like bus.pick_up(self, passenger_1)
 - Add a method that drops off a passenger and removes them from the list. This could look like bus.drop_off(self, passenger_2)
 - Add an 'empty' method to remove all of the passengers - this might be used when the bus reaches its destination, or if the bus breaks down. It should remove all of the passengers from the list.


Part 3
 - Create a new class called BusStop. This should have a name attribute.
 - Add an attribute to the BusStop called 'queue'. This should be an empty list that will get filled with instances of the Person class.
 - Add a method that adds a person to the queue.
 - Now imagine that our bus is travelling along the route. For now we will imagine that there is only one bus that goes on this route, so every passenger waiting at each stop wants to get on the bus.
 - Try writing a method that the bus would call, to collect all of the passengers from a stop. This might look like bus.pick_up_from_stop(self, bus_stop_1). This should take all of the passengers waiting in line at the stop, and put them inside of the bus. So the stop will now have nobody in the queue, and the number of people on the bus will increase by however many people the stop had at it.

Advanced Extension
 - Allow the passengers to have different destinations, so they only get on a bus which is going to that destination. So if they are at a bus stop and the wrong bus appears, they do not get on the bus. Write tests and functionality for this. (NOTE: you may need to change the functionality of some of your existing methods to allow for this)
