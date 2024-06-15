# ML-Driven Optimization of Childcare Allocation and Labor Demand 
This is the result of a project that utilized and applied public data related to daycare centers and labor (recruitment, job search) to machine learning algorithms.    

This result was also applied to the "2024 National Happiness Service Discovery and Entrepreneurship Contest" hosted by the Korea Social Security Information Service and was selected as the final entry.

[Contest Link](https://www.ssis.or.kr/lay1/bbs/S1T67C95/A/102/view.do?article_seq=125799&cpage=1&rows=10&condition=&keyword=)

## Motivation
In a situation where orphanage leavers and those requiring guardians continue to experience economic difficulties, and in South Korea, where labor shortages are worsening as we enter a super-aging society, the introduction of a job matching system for orphanage leavers is an urgent task.

## Output
Step 1. Data Curation (Reference to Data Source)</br></br>
Step 2. Data Preprocessing (Reference to algorithm)</br></br>
Step 3. Modeling </br>

- #1. Perform regional latitude/longitude-based clustering using the KMeans algorithm </br>
<img width="452" alt="그림1" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/e458c6df-a820-48ad-9f52-195c60e54d0b"> </br>


- #1. Using KMeans algorithm </br>
- #2. Perform clustering based on cluster latitude/longitude and labor values </br>
<img width="452" alt="그림2" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/548f621a-0517-4d71-92f3-43bf14cc9df1"> </br>


Step 4. Analysis and visualization </br>

- By looking at the visualized data, you can see which regions have a low labor demand ratio. </br>
- Therefore, population should be allocated to these regions first. </br>
<img width="452" alt="그림3" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/c426552d-7d74-4470-acc6-2920c49f1822"> </br>


Step 5. Childcare facility matching</br>

- Distance calculation </br>
<img width="452" alt="그림4" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/f06ae4bf-b01b-49f9-9dd0-64695f602ed1"> </br>


- Ranking calculation (Column(From Left): Labor figures_cluster, arrangement) </br>
<img width="114" alt="그림5" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/a1a685b7-2896-48f6-a732-2b242eab4db5"> </br>


## Algorithm
<img width="352" alt="그림6" src="https://github.com/joon-hee-kim/ML-Driven-Optimization-of-Childcare-Allocation-and-Labor-Demand/assets/121689436/56aa5a15-3bd2-47c6-b7d2-bf595448166d"> </br>

In the case of clustering, **k-means clustering** was used. For distance calculation, **KNN (K-Nearest Neighbors)** was employed. Data preprocessing was conducted using job opening and job application data from each region.

Labor Demand Ratio: This was calculated by dividing the number of job applications by the number of job openings. A lower value indicates a more severe labor supply shortage.
Required Workforce: This is an additional column added arbitrarily, representing the number of workers needed by subtracting the number of job applications from the number of job openings.


## 👥 Team Member

201934219 Kim Joonhee </br>

202031503 Kang Jiwon </br>

202034305 Kim Dabin </br>

202031512 Kim Minjae </br>

 
## ✔️ Data Source
Data Name: Status of child welfare facilities in 2022.  (Ministry of Health and Welfare) </br>
* List of Child Welfare Facilities in Seoul (Source: Seoul Open Data Plaza): [Data Link](https://data.seoul.go.kr/dataList/OA-20420/S/1/datasetView.do)
* Status of Child Care Facilities (Source: Gyeonggi Data Dream): [Data Link](https://data.gg.go.kr/portal/data/service/selectServicePage.do?page=1&rows=10&sortColumn=&sortDirection=&infId=VM9U79G9GCT38059YX9M12361361&infSeq=1&order=&loc=&searchWord=%EC%95%84%EB%8F%99+%EC%96%91%EC%9C%A1%EC%8B%9C%EC%84%A4+%ED%98%84%ED%99%A9)
* Busan Child Care Facilities (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/3076473/openapi.do)
* Daegu Child Welfare Facilities (Source: Daegu Metropolitan City Website): [Data Link](https://www.daegu.go.kr/woman/index.do;jsessionid=FACDD17BA231BF2BA14904508E7A6FC1.tomcat2?menu_id=00050130&servletPath=%2Fwoman)
* Incheon Metropolitan City_Child Welfare Facilities (Statistics)_20221231 (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/15064922/fileData.do)
* Gwangju Metropolitan City_Child Care Facilities Status_20231124 (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/15043858/fileData.do)
* Daejeon Child Care Facilities (Source: Daejeon Metropolitan City Child Association of Child Welfare): [Data Link](http://www.djchild.or.kr/page/facilities.php?device=pc)
* Sejong Child Welfare Facilities Status (As of April 2023) (Source: Sejong City): [Data Link](https://www.sejong.go.kr/bbs/R0595/view.do?nttId=B000000089056Kp1tB1f&mno=sub01_0101&cmsNoStr=&kind=&pageIndex=1)
* Chungcheongbuk-do Child Welfare Facilities (Source: Chungcheongbuk Province Government): [Data Link](https://www.chungbuk.go.kr/www/contents.do?key=4793)
* Chungcheongnam-do Child Care Facilities (Source: adongbokji): [Data Link](http://www.adongbokji.or.kr/adong/m/html/2_1.asp?page=2&address_1=%C3%E6%B3%B2&gubun2=&keyword1=&PB=%C8%B8%BF%F8%BD%C3%BC%B3%B0%CB%BB%F6#gotop)
* Jeollanam-do Child Care Facilities (Source: Jeonnam Association of Child Welfare): [Data Link](http://jn-adong.co.kr/bbs/sub_page_02.php)
* Gyeongsangbuk-do_Child Care Facilities Status_20231208 (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/15063057/fileData.do)
* Gyeongsangnam-do_Child Care Facilities_20221231 (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/15068287/fileData.do)
* Gangwon-do Child Care Facilities (Source: Korea Child Welfare Facilities): [Data Link](http://www.adongbokji.or.kr/adong/m/html/2_1.asp?PB=%C8%B8%BF%F8%BD%C3%BC%B3%B0%CB%BB%F6&address_1=%B0%AD%BF%F8#gotop)
* Jeju Special Self-Governing Province_Child Care Facilities Status_20230803 (Source: Public Data Portal): [Data Link](https://www.data.go.kr/data/3083487/fileData.do)
* Jeollabuk-do Child Care Facilities (Source: adongbokji): [Data Link](http://www.adongbokji.or.kr/adong/m/html/2_1.asp?page=2&address_1=%C0%FC%BA%CF&gubun2=&keyword1=&PB=%C8%B8%BF%F8%BD%C3%BC%B3%B0%CB%BB%F6#gotop)
* Number of Children in Need by Gender and Placement (202201~202212) (Source: Bokjiro): [Data Link](https://www.bokjiro.go.kr/ssis-tbu/twatga/sociGuaStat/SociGuaStatDetailIframe.do?datsNo=45&datsClNo=1051&datsClCrit=WS)

Data Name: Labor market status_recruitment_recruitment, job search, placement, employment status (Source: Korea Employment Information Service) [Data Link](https://www.data.go.kr/data/15067938/fileData.do?recommendDataYn=Y) </br>


