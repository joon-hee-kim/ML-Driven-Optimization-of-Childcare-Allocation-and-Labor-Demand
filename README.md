# ML-Driven Optimization of Childcare Allocation and Labor Demand 
This is the result of a project that utilized and applied public data related to daycare centers and labor (recruitment, job search) to machine learning algorithms.    

This result was also applied to the "2024 National Happiness Service Discovery and Entrepreneurship Contest" hosted by the Korea Social Security Information Service and was selected as the final entry.

[Contest Link](https://www.ssis.or.kr/lay1/bbs/S1T67C95/A/102/view.do?article_seq=125799&cpage=1&rows=10&condition=&keyword=)

## Motivation
In a situation where orphanage leavers and those requiring guardians continue to experience economic difficulties, and in South Korea, where labor shortages are worsening as we enter a super-aging society, the introduction of a job matching system for orphanage leavers is an urgent task.

## Output
- 1. Data Curation (explained below)</br>
- 2. Data Preprocessing (explained below)</br>
- 3. Modeling </br>
- #1. Perform regional latitude/longitude-based clustering using the KMeans algorithm
<img width="452" alt="그림1" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/e458c6df-a820-48ad-9f52-195c60e54d0b">

#1. Using KMeans algorithm 
#2. Perform clustering based on cluster latitude/longitude and labor values
<img width="452" alt="그림2" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/548f621a-0517-4d71-92f3-43bf14cc9df1">

- 4. Analysis and visualization </br>
By looking at the visualized data, you can see which regions have a low labor demand ratio. Therefore, population should be allocated to these regions first.
<img width="452" alt="그림3" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/c426552d-7d74-4470-acc6-2920c49f1822">

- 5. Childcare facility matching</br>
Distance calculation
<img width="452" alt="그림4" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/f06ae4bf-b01b-49f9-9dd0-64695f602ed1">

Ranking calculation
<img width="114" alt="그림5" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/a1a685b7-2896-48f6-a732-2b242eab4db5">

## Algorithm
<img width="352" alt="그림6" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/56aa5a15-3bd2-47c6-b7d2-bf595448166d">

## 👥 Team Member

201934219 Kim Joonhee </br>

202031503 강지원 </br>

202034305 김다빈 </br>

202031512 김민재 </br>

 
## ✔️ Data Source
Data Name: Status of child welfare facilities in 2022.  (Ministry of Health and Welfare)
Link:
Data Name: Labor market status_recruitment_recruitment, job search, placement, employment status (Korea Employment Information Service)
[Link](https://www.data.go.kr/data/15067938/fileData.do?recommendDataYn=Y)


