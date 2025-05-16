# THA_Dataset_Data_sample

**Exercise 3. EDA / Python:**
The purpose of this case study is to test your ability to leverage data to generate
useful insights.
Attached in THA_Dataset_Data_sample.csv you will find data corresponding to all
orders which happened during one
week (Delivered and Canceled) in the city of Glovalia with all important time

References. Note that:
- Store_address_id is the unique id identifying which store the order was for
- Courier_id is the id of the last courier the order was assigned to
-  Vertical
       -  ALL - Partner means the order was for a store which is our partner (they receive the orders through the partner web-app before the courier arrives there.
       -  ALL - NonPartner means the order was for a store which we have as “Fake” (we have no agreements with this store, so the courier needs to go inside and order as a regular customer).
-  QUIERO means the order was done through the central “Anything” button on the app where customers can ask us to deliver anything that fits into a Glovo backpack. (operationally similar to the WALL-NonPartner)
-  Transport is the vehicle type that was used by the courier who was assigned the last to the order
-  Activation is when the order enters the pool of active orders that need to be assigned to a courier.
● Number of assignments shows how many times we needed to assign
different couriers to the orders (e.g. if it is equal to 2, it means that the first
courier assigned refused to do the order and we needed to find a second
courier, in other words the order was reassigned)
● Total distance stands for the total real distance in KM the courier did to deliver
the order
Questions:
1. Based on the data you were given, provide visibility over the following metrics:
a. Delivery Time
b. Delivery Distance
c. Reassignment Rate (whenever we need to assign an order to another
courier after the first assignment it counts as a reassignment)
d. Courier Capacity (how many orders, on average, a courier is able to
deliver deliver during 1h of work)
e. Waiting time at pickup (time between arrival and the store,
“courier_enters_pickup”
, and picking up the order,
“pickup_time”)
2. Regarding reassignments can you see any trends / correlation with other
metrics?
3. Once the courier arrives at the store, the time until the order is picked-up
(waiting time at pickup), can present high variation. With the data given,
present an analysis showcasing this. Can you identify any clear trends in terms
of worst offenders? What could be the possible causes when the courier is
waiting for a very long time before picking up the order?
We encourage you to use Python and any module/package you see fit to solve the
exercise. We expect you to share with us the code used to import, clean and
transform the data as well as the calculations, plots and thought processes that
allowed you to reach your conclusions.
