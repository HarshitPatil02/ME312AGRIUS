The first four lines of the code install solvers such as gurobipy and cbc for subsequent code run

Temperature and pH are taken in as inputs through the website, and these inputs are used to filter through a CSV file containing the actual crops available for germination under these inputs

Fertilizer

Generating required n,p,k, and water level, saving them to water_crop_data.csv

Next, we take the present n,p,k, and water level data and take the difference with the required data

we then use the CBC solver to optimize the water distribution using the objective function and constraints

Now, for the fertilizer, we find the desired n,p, and k with respect to k, then normalize the n and p.
Then we find the (normalized N/N)/(normalized P/P) ratio and then compare the ratio with the CSV file containing the ideal fertilizer ratios

we also take into account the total cost per crop for fertilizer(total_fertilizer_per_crop)

We then go towards the pesticide optimization, in this we are assuming that the maximum possible yield is 80%, and for every gram of pesticide, the yield increases by 0.008 percent.
we then save this data to pesticide_usage.csv

We then move towards the labour_cost, and the maths has been displayed for this as well

We finally display the total_cost for each crop, the total_yield and the final_price

We then display the crop with maximum profits and the potential profits

The sustainability index is calculated and displayed

The crop rotation code provides us with the desired crop pairs available
