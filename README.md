# Mexican Restaurant Ratings Analysis
## Case Study
This project analyzes restaurant ratings in Mexico from real consumer feedback collected in 2012. It explores how consumer demographics, preferences, and behaviors influence their dining experiences. The dataset includes detailed information on consumers, restaurants, cuisines, and satisfaction ratings. Using Power BI, the analysis uncovers patterns in food, service, and overall satisfaction, providing valuable insights into regional dining trends and customer expectations.
## Data Description
The dataset is structured around five key entities: **Consumers**, **Consumer Preferences**, **Ratings**, **Restaurants**, and **Restaurant Cuisines**. Below is a brief overview of the variables included in each:
#### 👤 **Consumers**
- `Consumer_ID`: Unique identifier for each consumer  
- `City`: City of residence  
- `State`: State of residence  
- `Country`: Country of residence  
- `Latitude`: Geographical latitude of the consumer  
- `Longitude`: Geographical longitude of the consumer  
- `Smoker`: Indicates whether the consumer smokes  
- `Drink_Level`: Indicates if the consumer is an abstemious, casual, or social drinker  
- `Transportation_Method`: Preferred method of transport (on foot, public transport, or car)  
- `Marital_Status`: Marital status (single or married)  
- `Children`: Indicates presence of dependent or independent children  
- `Age`: Age of the consumer  
- `Occupation`: Employment status (student, employed, or unemployed)  
- `Budget`: Consumer’s budget category (low, medium, high)

---

#### 🍽️ **Consumer Preferences**
- `Consumer_ID`: Unique identifier for each consumer  
- `Preferred_Cuisine`: Type(s) of cuisine the consumer prefers

---

#### ⭐ **Ratings**
- `Consumer_ID`: Unique identifier for each consumer  
- `Restaurant_ID`: Unique identifier for each restaurant  
- `Overall_Rating`: Overall experience rating (0 = Unsatisfactory, 1 = Satisfactory, 2 = Highly Satisfactory)  
- `Food_Rating`: Rating for the food quality  
- `Service_Rating`: Rating for the service quality

---

#### 🏢 **Restaurants**
- `Restaurant_ID`: Unique identifier for each restaurant  
- `Name`: Name of the restaurant  
- `City`: City where the restaurant is located  
- `State`: State where the restaurant is located  
- `Country`: Country where the restaurant is located  
- `Zip_Code`: Postal code of the restaurant  
- `Latitude`: Geographical latitude of the restaurant  
- `Longitude`: Geographical longitude of the restaurant  
- `Alcohol_Service`: Type of alcohol service (none, wine & beer, full bar)  
- `Smoking_Allowed`: Smoking policy (none, in bar, in designated sections)  
- `Price`: Price level of the restaurant (low, medium, high)  
- `Franchise`: Indicates whether the restaurant is a franchise  
- `Area`: Restaurant environment (open or closed area)  
- `Parking`: Availability of parking (none, yes, public, valet)

---

#### 🍕 **Restaurant Cuisines**
- `Restaurant_ID`: Unique identifier for each restaurant  
- `Cuisine`: Type(s) of cuisine offered by the restaurant

## ER Diagram
![image](https://github.com/user-attachments/assets/4ec0974b-048e-494f-a426-e8c56c730127)

## Data Analysis

### 🏙️ **Local Insights**

**1. What is the distribution of consumers by city and state?**  
The highest concentration of consumers is found in Tijuana, Baja California. Valladolid, Yucatan follows as the second most populous consumer location.

**2. How prevalent is parking availability at restaurants in different cities?**  
Most restaurants across the cities lack parking facilities. In Tijuana and Valladolid, valet parking is available at few restaurants. Public parking is accessible in Acapulco, Tijuana, and Valladolid.

**3. How does the age distribution of consumers vary by state?**  
Across all three states, the majority of consumers are young adults under 30 years old. In Baja California and Yucatan, seniors over 60 represent the second largest age group.

**4. What percentage of consumers are smokers or non-smokers in each city?**  
Most consumers in all four cities are non-smokers. Merida has a 100% non-smoking population, while Tijuana has the highest proportion of smokers, accounting for 25%.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .  

### 🍽️ **Dining Insights**

**1. How does parking availability relate to restaurant price levels?**  
All 24 high-priced restaurants offer some form of parking, three provide valet, one offers public parking, and five lack dedicated parking. Medium and low-priced restaurants do not offer valet service but may provide public or private parking depending on the establishment.

**2. How do consumer ratings compare between franchise and non-franchise restaurants?**  
Non-franchise restaurants dominate the dataset and are evenly spread across all rating categories—unsatisfactory, satisfactory, and highly satisfactory. Franchise restaurants, though fewer, show a similar balanced distribution.

**3. What is the distribution of restaurants by state?**  
Baja California hosts the largest number of restaurants (84), while Yucatan and Guerrero each have 23.

**4. What cuisines are most preferred based on consumer demographics?**  
Mexican cuisine is the most popular across all consumer profiles, followed by American cuisine.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .  

### 🥂 **Hospitality Insights**

**1. What are the most common modes of transportation among consumers?**  
Public transportation is the most widely used method of consumers. This is followed by car usage and walking.

**2. What proportion of restaurants allow smoking in each state?**  
Approximately 95 restaurants enforce smoke-free policies. Around 9 allow smoking, and 24 offer designated smoking areas. A very small number permit smoking in bar sections, specifically in Baja California and Yucatan.

**3. How does alcohol service vary across restaurants in different cities?**  
Among restaurants in Acapulco, Merida, Tijuana and Valladolid, 66.92% do not serve alcohol. Approximately 26.15% offer wine and beer, and only 6.93% feature a full bar.

**4. How does alcohol service influence consumer satisfaction ratings?**  
Non-drinkers gave 303 "highly satisfactory" ratings, 289 "satisfactory," and 170 "unsatisfactory." Consumers at wine-and-beer-serving restaurants gave 146 "highly satisfactory" ratings. Full bar establishments received 37 "highly satisfactory" ratings, 27 "satisfactory," and 16 "unsatisfactory."

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .  

### 👥 **Behavioral Insights**

**1. Is there a relationship between occupation and budget level?**  
Most students report having a medium budget (67), followed by low (33), and a few with high budgets (4). Among employed individuals, 15 report a medium budget, while one unemployed individual also falls into the medium budget category.

**2. How does marital status relate to smoking and drinking habits?**  
Among 88 single consumers, all are non-smokers, and their drinking preferences range from abstemious to social. Among married non-smokers, two are abstemious and five are social drinkers. There are also 23 single smokers who tend to be either casual or social drinkers. Two married smokers are also social drinkers.

**3. How do drinking habits vary across states?**  
In Baja California, 31 are social drinkers, 28 casual, and 18 abstemious. Guerrero has 10 abstemious, 6 casual, and 3 social drinkers. In Yucatan, there are 11 abstemious, followed by 10 casual and 3 social drinkers.

**4. What are the most common occupations among consumers in each state?**  
In Baja California, students make up 93% of the consumer population. Yucatan has an even mix of students and employed individuals. In Guerrero, 94% are students, with a small percentage being employed.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .  

### 🏆 **Review Insights**
**1. Which restaurants have the highest food ratings?**
Top-rated for food satisfaction include Mision 19 and Telephonica Gastro Park, where most customers rated their food as "highly satisfactory." Caesar's Restaurant received 9 high ratings, La Justina received 10, and Tocas El Franc earned 11.

**2. Which restaurants have the highest service ratings?**
Mision 19 leads in service satisfaction, followed by Telephonica Gastro Park and Caesar's Restaurant, each with 12 "satisfactory" ratings.La Justina also has 12 satisfied ratings, while Tocas El Franc received 7.

**3. Which restaurants have the highest overall ratings?**
Mision 19 and Telephonica Gastro Park top the list, with the latter receiving 30 "highly satisfactory" ratings. Caesar's Restaurant earned 24, Tocas El Franc 28, and Restaurant La Chalita follows with 20.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .  

![Screenshot 2025-04-18 133950](https://github.com/user-attachments/assets/9f895e46-08f0-48be-839d-efdaa9e27fcb)

![image](https://github.com/user-attachments/assets/24bbb820-2fbd-4bc3-bca8-74206f33e39c)

![image](https://github.com/user-attachments/assets/8660387c-faf4-4990-a8a2-287eacf4f443)

![image](https://github.com/user-attachments/assets/55310f8c-9348-4480-a984-885618216dce)

![image](https://github.com/user-attachments/assets/7aba3634-f2ab-4b30-966f-4362bd2e36a7)











