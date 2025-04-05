# OPTIMIZATION-MODEL

COMPANY: CODTECH IT SOLUTIONS

NAME: GURRALA LAXMI PARIMAL

INTERN ID: CT12RER

DURATION: 8 WEEKS

MENTOR: NEELA SANTHU

##Description: This Python script performs a supply chain optimization task using linear programming, aimed at minimizing total transportation costs while fulfilling customer demand and respecting warehouse supply constraints. The core objective is to determine the most cost-effective way to distribute goods from multiple warehouses to multiple customers. This kind of optimization is essential in logistics and supply chain management, where businesses must balance supply capabilities with customer demand, all while minimizing operational expenses.
The script uses the PuLP library, a Python package specifically designed for linear programming. It allows users to define optimization problems, variables, constraints, and objective functions in a programmatic and readable way. In this particular scenario, three warehouses (W1, W2, W3) and three customers (C1, C2, C3) are defined, along with the available supply at each warehouse and the demand at each customer location. The costs of transporting goods from each warehouse to each customer are also specified in a dictionary.
To model this as a linear programming problem, a decision variable is created for each pair of warehouse and customer, representing the number of units to ship between them. These variables are continuous and non-negative, reflecting real-world logistics scenarios where shipments can be fractional or measured in bulk units. The objective function is to minimize the total transportation cost, which is the sum of the product of each shipment quantity and its corresponding cost.
Two types of constraints are added to the model. First, supply constraints ensure that the total quantity shipped from any warehouse does not exceed its available inventory. Second, demand constraints ensure that each customer receives at least the required quantity of goods. These constraints reflect realistic operational limitations in logistics, such as inventory capacities and guaranteed service levels to customers.
Once the model is defined, it is solved using the default solver provided by PuLP. The script prints the status of the solution (e.g., Optimal) and the total minimized cost. It also extracts the optimized shipping quantities and organizes them into a structured DataFrame using the pandas library. This final table clearly shows how many units should be shipped from each warehouse to each customer to achieve the lowest total cost while meeting all supply and demand requirements.
The development and execution of this model are done entirely in Python, leveraging key packages like pandas for data handling and PuLP for optimization modeling. The script includes optional pip installation commands to ensure that dependencies such as numpy, pandas, bottleneck, and PuLP are installed and up to date. This makes the code portable and reproducible across environments.
In terms of platforms, this code is well-suited to be run in any Python-supported environment, such as Jupyter Notebooks, local IDEs like PyCharm or VS Code, or cloud-based notebooks such as 
Google Colab or Kaggle Kernels. It is especially useful in academic settings, operational research, and industries focused on logistics, distribution, and resource allocation. Overall, this script demonstrates the power of mathematical modeling combined with Python’s ecosystem for solving real-world optimization problems in a practical, scalable, and cost-effective manner.
