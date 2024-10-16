**Constructive Cost Model (COCOMO)** is used in estimating the cost, effort, and schedule for software development projects. 

Developed by *Barry Boehm* in the early 1980s, COCOMO provides a structured approach to project estimation based on the size of the software being developed.

### 1.There are three types of Models 
    1.Basic
        organic :  For small and  simple projects with a small team.
        semi-detached :  For medium-sized projects , deals with some complexity.
        embedded : For large, complex projects with tight constraints.          
    
    2.Intermediate
        Expands on the basic model by incorporating cost drivers such as product attributes, hardware attributes, personnel attributes,and project attributes.

    3.Detailed
        It further enhances the intermediate COCOMO,providing more detailed estimates by considering phases of development (e.g., design,coding, testing).


**2.Project size (KLOC)**: Kilo lines of code . Generally we estimate the size of kloc based on the mode that we choose should also consider the strict rules for reliability, testing, and following regulations while choosing kloc.

**Cost Drivers**: 
    Intermediate cocomo model states that the amount of work needed to create a software depends on the number of lines of code and has fixed constants for different softwares. In reality, our code can't estimate time and work. There are other important factors, such as software performance and team experience. Cost Drivers are 15 important factors used by the intermediate model to estimate cost.

#####  Cost Drivers and their attributes 

*Product attributes, Hardware attributes , Personal attributes , Project attributes and platform attributes*

some attributes are given below for reference

Product attributes : Required Software Reliability , Product Complexity

Computer  attributes:Execution Time Constraint ,storage constraints

Personnel Attributes: Programmer capability, Personnel/project Experience 

Project Attributes : Modern Programming languages, Tools 

Estimation Formula: The basic formula for estimating effort in person-months is:
        
        Effort (PM)=a×(KLOC)^b 

a and b are constants that vary based on the project mode (Organic, Semi-Detached, Embedded).
![alt text](<Screenshot 2024-10-16 at 11.20.47 AM.png>)

in the above example we have a = 4.498, 50 kloc and b = 1.12

Effort (PM)=4.498×(50) ^ 1.12

Effort (PM)=4.498×79.9551≈359.6382

The estimated effort for the project would be approximately **359 person-months**.
Duration: 
        +Duration (months)=c*effort^d 
        +Duration (months) =    * 359.6382 ^ 0.32
        +Duration (months) =  2.5  * 7.8442790615432
        +Duration (months ) = 19.611
Staffing : 
        Staffing = effort / duration 
        Staffing = 359.6382 / 19.611
        Staffing = 18.340

#### What can this model do ?
It can provide an estimate for Total effort in person-months , Schedule in months , Required team size 

#### where is this model primarily used at ?
COCOMO is widely used for project planning, budgeting, and resource allocation in software development. It helps project managers and stakeholders understand the potential costs and timeframes, facilitating better decision-making.

