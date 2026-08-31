Student Enrollment Management & Analytics Dashboard

📊 Project Overview

Mashruucan waa Student Enrollment Management & Analytics Dashboard
oo lagu falanqeeyay xog ardayeed iyadoo la adeegsanayo Microsoft
Excel.

Ujeeddada mashruucu waa in xogta enrollment-ka laga sameeyo:

Data Cleaning iyo Data Quality Analysis

Pivot Tables

Pivot Charts

KPIs

Interactive Slicers

Enrollment Dashboard

Tuition iyo enrollment analysis

Mashruucu wuxuu isku daraa xogta ardayda, enrollment status, study mode,
program, gender, enrollment date iyo tuition fee si loo helo warbixin si
fudud loo fahmi karo.

🎯 Project Objectives

Mashruucan waxaa looga gol leeyahay:

In la ogaado tirada guud ee ardayda.

In la falanqeeyo Enrollment Status.

In la barbar dhigo Gender.

In la fahmo Study Mode ee ardayda.

In la ogaado barnaamijyada ardaydu ugu badan yihiin.

In la falanqeeyo Tuition Fee ee program kasta.

In la eego enrollment-ka iyadoo loo eegayo taariikhda.

In la ogaado khaladaadka iyo missing values-ka xogta.

In xogta loogu beddelo dashboard interactive ah.

🧹 Data Cleaning & Data Quality

Qaybta analysis-ka waxaa lagu ogaaday in dataset-ku leeyahay qaar ka mid
ah xog aan sax ahayn ama maqan.

Gender

Gender          Count

Male              148
Female            136
Blank              15
Non-value           1
Total     300

Program Data Quality

Waxaa jira values u baahan standardization ama sixid, sida:

BA

CS

NULL

Unknown

blank

non_program

Waxaa sidoo kale muuqda values sax ah sida:

Business Administration

Computer Science

Data Science

Economics

Engineering

Public Health

Study Mode

Study Mode-ka waxaa ka muuqda values kala duwan:

Full-Time

Part-Time

Online

N/A

NULL

Blank

non_stady_mode

non_stady_mode waa value u baahan in la standardize gareeyo ama loo
beddelo category sax ah.

Enrollment Status

Enrollment Status-ka waxaa jira:

Active

Deferred

Graduated

Withdrawn

N/A

Blank

non_status

Waxaa muhiim ah in values-ka khaldan ama maqan la nadiifiyo ka hor
analysis-ka ugu dambeeya.

Duplicate Student IDs

Analysis-ka wuxuu muujiyay in qaar ka mid ah Student_ID ay soo
noqnoqdaan. Tusaale ahaan waxaa jira Student IDs leh count 2, taas
oo u baahan in la hubiyo haddii ay yihiin duplicate dhab ah ama records
sax ah.

Missing Student IDs

Waxaa sidoo kale jira records leh Student_ID ka maqan. Sidaa darteed
Student_ID waa field muhiim ah oo loo baahan yahay in la hubiyo.

📌 Pivot Tables & Analysis

1. Enrollment Status

Pivot Table-ka Enrollment Status wuxuu muujiyay:

Enrollment Status            Students

Active                            175
Deferred                           27
Graduated                          64
Withdrawn                          16
Total shown in pivot      282

Chart-ka waxaa loo adeegsaday in si muuqata loo barbar dhigo status-yada
ardayda.

Insight: Active students ayaa ah kooxda ugu badan, halka Deferred
iyo Withdrawn ay yihiin kooxaha ugu yar.

Fiiro gaar ah: dataset-ka guud wuxuu leeyahay 300 records, laakiin
pivot-kan wuxuu tirinayaa Tuition_Fee, sidaas darteed total-ku waa
282. Records-ka Tuition_Fee ka maqan laguma darin count-kan.

2. Enrollment Date

Enrollment Date analysis-ka waxaa lagu sameeyay Pivot Table iyo Line
Chart.

Waxaa lagu arkay counts kala duwan oo ay ka mid yihiin:

18

26

23

34

20

6

10

55

78

30

Waxaa jira #VALUE! oo ka muuqda date grouping-ka, taasoo tilmaamaysa
in qaar ka mid ah Enrollment Date values aysan ahayn dates sax ah ama ay
leeyihiin data-type problem.

Recommended Fix

Enrollment Date waa in:

La hubiyaa in dhammaan values-ku yihiin Excel Date.

#VALUE! iyo invalid dates la saxo.

Column-ka loo format-gareeyo Date.

Kadib Pivot Table-ka lagu sameeyo Group by Months/Years.

3. Study Mode

Pivot Table-ka Study Mode:

Study Mode         Students

Full-Time               162
Part-Time                59
Online                   60
non_stady_mode           19
Total           300

Pie Chart-ka wuxuu muujinayaa distribution-ka Study Mode.

Insight: Full-Time ayaa leh tirada ugu badan ee ardayda, halka
non_stady_mode uu yahay category u baahan cleaning.

4. Tuition by Program

Tuition-ka waxaa lagu falanqeeyay Program kasta:

Program                              Tuition

Business Administration          $36,617.50
Computer Science                 $68,526.92
Data Science                     $65,662.73
Economics                        $19,402.25
Engineering                      $42,936.93
non_program                      $17,318.41
Public Health                    $30,457.95
Total                   $280,922.69

Key Insight

Computer Science ayaa leh tuition-ka ugu sarreeya, waxaana ku xiga
Data Science.

📈 Dashboard

Dashboard-ka wuxuu isku daraa KPIs, charts iyo slicers si user-ku si
interactive ah ugu falanqeeyo xogta.

Main KPIs

Dashboard-ka waxaa loogu talagalay inuu muujiyo:

KPI                           Value

Total Students                  300
Active Students                 175
Graduated Students               64
Total Tuition          $280,922.69
Average Tuition            $996.18

⚠️ KPI Correction

Sawirka dashboard-ka waxaa ka muuqda Total Tuition oo lagu qoray
$996.18. Taasi waxay u muuqataa in formula-ga KPI-ga Total Tuition
uu si khaldan u isticmaalayo Average.

Qiimaha saxda ah ee Total Tuition waa:

$280,922.69

Average Tuition-na waa:

$996.18

Average-kan wuxuu ku salaysan yahay 282 records oo leh Tuition_Fee:

$280,922.69 ÷ 282 ≈ $996.18

Sidaas darteed labada KPI waa in loo kala saaraa:

Total Tuition → $280,922.69

Average Tuition → $996.18

📊 Dashboard Charts

Dashboard-ka waxaa ku jira charts muhiim ah:

1. Total Gender

Waxa uu muujinayaa tirada ardayda Male iyo Female, iyadoo sidoo kale
data quality-ga lagu arkayo blank/non-value records.

2. Tuition by Program

Horizontal Bar Chart ayaa lagu muujiyay tuition-ka program kasta.

3. Total Enrollment Status

Waxa uu muujinayaa:

Active

Deferred

Graduated

Withdrawn

non_status

4. Total Study Mode

Waxa uu muujinayaa:

Full-Time

Part-Time

Online

non_stady_mode

5. Enrollment Date

Line Chart ayaa loo adeegsaday in lagu muujiyo enrollment-ka iyadoo loo
eegayo date/month.

🎛️ Interactive Slicers

Dashboard-ka waxaa lagu daray Slicers si user-ku u filter-gareyn karo
dashboard-ka.

Slicers-ka waxaa ka mid ah:

Gender

Study_Mode

Program

Enrollment_Status

Enrollment_Date

Slicers-ku waxay dashboard-ka ka dhigayaan interactive, waxaana user-ku
dooran karaa category gaar ah si charts-ka iyo analysis-ku ula socdaan
filter-ka.

🔍 Key Findings

Waxaa laga helay analysis-ka:

Total records = 300 students.

Active = 175, waana enrollment status-ka ugu badan.

Graduated = 64.

Deferred = 27.

Withdrawn = 16.

Full-Time = 162, waana Study Mode-ka ugu badan.

Online = 60.

Part-Time = 59.

Computer Science ayaa leh tuition-ka ugu badan, qiyaastii
$68.5K.

Data Science ayaa ku xigta, qiyaastii $65.7K.

Total Tuition-ka la muujiyay waa $280,922.69.

Average Tuition-ka records-ka Tuition_Fee leh waa qiyaastii
$996.18.

Dataset-ka waxaa ku jira missing values, invalid values, duplicates
iyo inconsistent categories.

Enrollment Date column-ka waxaa ka muuqda #VALUE!, sidaas darteed
date cleaning ayaa loo baahan yahay.

🛠️ Excel Skills Used

Mashruucan wuxuu ku tababarayaa xirfadaha Excel ee muhiimka ah:

Data Cleaning

Remove Duplicates

Handling Blank Values

Data Validation

Data Formatting

Pivot Tables

Pivot Charts

Slicers

KPI Cards

SUM

COUNT

AVERAGE

Filtering

Sorting

Date Grouping

Dashboard Design

Data Quality Analysis

📁 Suggested Workbook Structure

Workbook-ka waxaa lagu habeyn karaa sidan:

Student_Enrollment_Project.xlsx
│
├── Raw_Data
├── Data_Clean
├── Pivot_Tables
├── Pivot_Charts
├── Analysis
└── Dashboard

Raw_Data

Xogta asalka ah.

Data_Clean

Xogta la nadiifiyay oo loo diyaariyay analysis.

Pivot_Tables

Pivot tables-ka kala duwan.

Pivot_Charts

Charts-ka laga sameeyay Pivot Tables.

Analysis

Data quality checks, duplicates, missing values iyo error checks.

Dashboard

Final interactive dashboard-ka.

🚀 Recommended Improvements

Si mashruucu u noqdo mid professional ah:

Sax Total Tuition KPI-ga.

Nadiifi #VALUE! ee Enrollment Date.

Standardize BA → Business Administration.

Standardize CS → Computer Science.

Hubi NULL, Unknown, blank iyo non-values.

Sax non_stady_mode haddii ay tahay typo.

Hubi duplicate Student IDs.

Samee Year/Month columns haddii date analysis loo baahan yahay.

Ku dar percentage KPIs sida:

Active Rate

Graduation Rate

Withdrawal Rate

Dashboard-ka ka dhig mid si buuxda ugu xiran Pivot Tables iyo
Slicers.

🏁 Conclusion

Mashruucani waa Student Enrollment Analytics Dashboard oo lagu
isticmaalo Excel si loo fahmo enrollment-ka ardayda, study mode, gender,
programs, enrollment status iyo tuition revenue.

Waxa ugu muhiimsan ee mashruucu muujinayo waa in data cleaning uu
yahay tallaabo muhiim ah ka hor inta aan la sameyn Pivot Tables iyo
Dashboard. Marka values-ka khaldan, blanks, duplicates iyo date errors
la saxo, dashboard-ku wuxuu bixin karaa analysis ka sax badan oo loogu
adeegsan karo go'aan qaadashada maamulka waxbarashada.

👨‍💻 Project Type

Microsoft Excel -- Data Cleaning, Pivot Tables, Pivot Charts &
Dashboard

Topic: Student Enrollment Management & Analytics

Status: Dashboard Completed --- Data Quality Improvements
Recommended
