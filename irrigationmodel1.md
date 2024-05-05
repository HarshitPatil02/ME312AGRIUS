This code demonstrates crop yield prediction and provides a simple irrigation optimization function based on water availability and crop water needs using a linear regression model.

Plots individual relationships between each feature and the target variable (crop yield) in separate subplots: Temperature vs. Crop Yield, Humidity vs. Crop Yield, and Rainfall vs. Crop Yield. Displays a 3D scatter plot illustrating the relationships between all three features (temperature, humidity, and rainfall) and the crop yield.

to find the optimal water application for maximizing crop yield while satisfying two constraints: total available water for irrigation and crop water requirements. The objective function, water constraint, and crop constraint values are calculated for the range of water values. These values are then plotted against the amount of water applied. The optimal water application is visualized using a vertical dashed red line.

water distribution across a 2D grid of crops to maximize crop yield while adhering to water constraints. grid_size: Defines the dimensions of the 2D grid. num_crops: Specifies the number of different crop types. crop_types: Assigns random crop types to each grid point. water_requirements: Assigns random water requirements to each crop type. Ensures that the total applied water does not exceed the total available water for irrigation.

Visualization of Initial and Optimal Water Distributions
