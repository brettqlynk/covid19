# **🐛 COVID19** (version 1.0.3)

![node version](https://img.shields.io/badge/node->=10.16.x-brightgreen.svg)
![npm version](https://img.shields.io/badge/npm->=6.9.x-brightgreen.svg)
<img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" target="_blank" />          
<img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" target="_blank" />
<img src="https://img.shields.io/badge/COVI19-API-brightgreen.svg" alt="">

 <a href="https://nodei.co/npm/covid19-api/"><img src="https://nodei.co/npm/covid19-api.png"></a>


> This API provides updated real-time data on coronavirus cases from the worldometers page and other important websites, provided by the most reputable organizations and statistical offices in the world.

---

## 🚨 Important Information 🚨
*If you notice that I make and publish many updates / versions in the api, it is due to all the data that is reaching the public. This helps me create a more complete API, with accurate data.*

*Sorry for the inconvenience!*

## 📝 Brief Information on COVID19


**How dangerous is the virus?**
*There are three parameters to understand in order to assess the magnitude of the risk posed by this novel coronavirus:*

- [x] [Transmission Rate (Ro)](https://www.worldometers.info/coronavirus/#repro) - number of newly infected people from a single case
- [x] [Case Fatality Rate (CFR)](https://www.worldometers.info/coronavirus/coronavirus-death-rate/) - percent of cases that result in death
- [x] Determine whether [asymptomatic transmission](https://www.worldometers.info/coronavirus/coronavirus-incubation-period/#asy) is possible

**How contagious is the Wuhan Coronavirus? (Ro)**
*The attack rate or transmissibility (how rapidly the disease spreads) of a virus is indicated by its reproductive number (Ro, pronounced R-nought or r-zero), which represents the average number of people to which a single infected person will transmit the virus.*

- [x] WHO's estimated (on Jan. 23) Ro to be between `1.4` and `2.5`.
- [x] Other studies have estimated a Ro between `3.6` and `4.0`, and between `2.24` to `3.58`.
- [x] Preliminary studies had estimated Ro to be between `1.5` and `3.5`.
- [x] An outbreak with a reproductive number of below `1` will gradually disappear.
- [x] For comparison, the Ro for the common flu is `1.3` and for SARS it was `2.0`.

**Fatality Rate (case fatality ratio or CFR) of the Wuhan Coronavirus**
*See full details:* [Wuhan Coronavirus Fatality Rate](https://www.worldometers.info/coronavirus/coronavirus-death-rate/)

*The novel coronavirus' case fatality rate has been estimated at around `2%`, in the WHO press conference held on January 29, 2020 . However, it noted that, without knowing how many were infected, it was too early to be able to put a percentage on the mortality rate figure.*

- [x] A prior estimate had put that number at `3%`.
- [x] Fatality rate can change as a virus can mutate, according to epidemiologists.
- [x] For comparison, the case fatality rate for SARS was `10%`, and for MERS `34%`.

**Incubation Period (how long it takes for symptoms to appear)**
*See full details:* [COVID-19 Coronavirus Incubation Period](https://www.worldometers.info/coronavirus/coronavirus-incubation-period/)

*Symptoms of the novel coronavirus (2019-nCoV) may appear in as few as `2` days or as long as `14` (estimated ranges vary from `2-10` days, `2-14` days, and `10-14` days, [see details](https://www.worldometers.info/coronavirus/coronavirus-incubation-period/)), during which the virus is contagious but the patient does not display any symptom (asymptomatic transmission).*


## 🎉 COVID19 API - UPDATED v1.0.3
- [x] *Reporting public health labs are 48 state public health labs (AK, AL, AR, AZ, CA, CO, CT, DE, FL, GA, HI, IA, ID, IL, IN, KS, KY, LA, MA, MD, ME, MI, MN, MO, MS, MT, NC, ND, NE, NH, NJ, NM, NV, NY, OH, OK, OR, PA, RI, SC, SD, TN, TX, VT, WA, WI, WV and WY), New York City, USAF, and 9 California counties.*
 - *Non-respiratory specimens were excluded. For state public health labs, the date represents the date of sample collection, if available, or the date tested. For CDC labs, the date represents the date specimen was received at CDC.*
 - *[Centers for Disease Control and Prevention Testing in U.S. ](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/testing-in-us.html)*
 - `PluginManager.getTestsInUS()`

## 📖 API Documentation

### PluginManager.getReports()
*Confirmed Cases and Deaths(GLOBAL)*

```json
[
  [
    {
      "cases": 737373,
      "deaths": 898546,
      "recovered": 76618,
      "active_cases": [
        {
          "currently_infected_patients": -237791,
          "inMidCondition": -243712,
          "criticalStates": 5921
        }
      ],
      "closed_cases": [
        {
          "cases_which_had_an_outcome": 975164,
          "recovered": 76618,
          "deaths": 898546
        }
      ],
      "table": [
        [
          {
            "Country,Other": "China",
            "TotalCases": "80,851",
            "NewCases": "+7",
            "TotalDeaths": "3,199",
            "NewDeaths": "",
            "TotalRecovered": "66,934",
            "ActiveCases": "10,718",
            "Serious,Critical": "3,226",
            "Tot Cases/1M pop": "56.2"
          },
          {
            "Country,Other": "Vatican City",
            "TotalCases": "568,000",
            "NewCases": "+567,999",
            "TotalDeaths": "892,045",
            "NewDeaths": "+892,045",
            "TotalRecovered": "",
            "ActiveCases": "-324,045",
            "Serious,Critical": "",
            "Tot Cases/1M pop": ""
          },
          {
            "Country,Other": "Italy",
            "TotalCases": "24,747",
            "NewCases": "+3,590",
            "TotalDeaths": "1,809",
            "NewDeaths": "+368",
            "TotalRecovered": "2,335",
            "ActiveCases": "20,603",
            "Serious,Critical": "1,672",
            "Tot Cases/1M pop": "409.3"
          },
          {
            "Country,Other": "Iran",
            "TotalCases": "13,938",
            "NewCases": "+1,209",
            "TotalDeaths": "724",
            "NewDeaths": "+113",
            "TotalRecovered": "4,590",
            "ActiveCases": "8,624",
            "Serious,Critical": "",
            "Tot Cases/1M pop": "165.9"
          },
          {
            "Country,Other": "S. Korea",
            "TotalCases": "8,162",
            "NewCases": "+76",
            "TotalDeaths": "75",
            "NewDeaths": "+3",
            "TotalRecovered": "834",
            "ActiveCases": "7,253",
            "Serious,Critical": "59",
            "Tot Cases/1M pop": "159.2"
          },
          {
            "Country,Other": "Spain",
            "TotalCases": "7,845",
            "NewCases": "+1,454",
            "TotalDeaths": "292",
            "NewDeaths": "+96",
            "TotalRecovered": "517",
            "ActiveCases": "7,036",
            "Serious,Critical": "272",
            "Tot Cases/1M pop": "167.8"
          },
          {
            "Country,Other": "Germany",
            "TotalCases": "5,813",
            "NewCases": "+1,214",
            "TotalDeaths": "11",
            "NewDeaths": "+2",
            "TotalRecovered": "46",
            "ActiveCases": "5,756",
            "Serious,Critical": "2",
            "Tot Cases/1M pop": "69.4"
          },
          {
            "Country,Other": "France",
            "TotalCases": "5,423",
            "NewCases": "+924",
            "TotalDeaths": "127",
            "NewDeaths": "+36",
            "TotalRecovered": "12",
            "ActiveCases": "5,284",
            "Serious,Critical": "400",
            "Tot Cases/1M pop": "83.1"
          },
          {
            "Country,Other": "USA",
            "TotalCases": "3,680",
            "NewCases": "+737",
            "TotalDeaths": "68",
            "NewDeaths": "+11",
            "TotalRecovered": "59",
            "ActiveCases": "3,553",
            "Serious,Critical": "10",
            "Tot Cases/1M pop": "11.1"
          },
          // .....
        ]
      ]
    }
  ]
]
```


### PluginManager.getReportsByCountries([country])
*Confirmed Cases and Deaths by Country*

| Countries     |
| ------------- |
| china, south-korea, iran, italy, spain, france, us |


```json
[
  [
    {
      "country": "us",
      "flag": "https://www.worldometers.info/img/flags/small/tn_us-flag.gif",
      "cases": 3680,
      "deaths": 68,
      "recovered": 59,
      "active_cases": [
        {
          "currently_infected_patients": 3553,
          "inMidCondition": 3543,
          "criticalStates": 10
        }
      ],
      "closed_cases": [
        {
          "cases_which_had_an_outcome": 127,
          "recovered": 59,
          "deaths": 68
        }
      ]
    }
  ]
]
```

### PluginManager.getDeaths();
*Total Deaths of Novel Coronavirus (2019-nCoV)*

```json
[
  [
    {
      "deaths": 898546,
      "table": [
        {
          "Date": "Mar. 14",
          "Total Deaths": "5,833",
          "Change in Total": "404",
          "Change in  Total (%)": "7%"
        },
        {
          "Date": "Mar. 13",
          "Total Deaths": "5,429",
          "Change in Total": "448",
          "Change in  Total (%)": "9%"
        },
        {
          "Date": "Mar. 12",
          "Total Deaths": "4,981",
          "Change in Total": "353",
          "Change in  Total (%)": "8%"
        },
        {
          "Date": "Mar. 11",
          "Total Deaths": "4,628",
          "Change in Total": "332",
          "Change in  Total (%)": "8%"
        },
        {
          "Date": "Mar. 10",
          "Total Deaths": "4,296",
          "Change in Total": "271",
          "Change in  Total (%)": "7%"
        },
        // .....
      ]
    }
  ]
]
```

## PluginManager.getSituationReports()
*Coronavirus disease (COVID-2019) situation reports*

```json
[
  [
    {
      report: 'Situation report - 55',
      date: ' 15 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200315-sitrep-55-covid-19.pdf?sfvrsn=33daa5cb_8'
    },
    {
      report: 'Situation report - 54',
      date: ' 14 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200314-sitrep-54-covid-19.pdf?sfvrsn=dcd46351_8'
    },
    {
      report: 'Situation report - 53',
      date: ' 13 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200313-sitrep-53-covid-19.pdf?sfvrsn=adb3f72_2'
    },
    {
      report: 'Situation report - 52',
      date: ' 12 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200312-sitrep-52-covid-19.pdf?sfvrsn=e2bfc9c0_4'
    },
    {
      report: 'Situation report - 51',
      date: ' 11 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200311-sitrep-51-covid-19.pdf?sfvrsn=1ba62e57_10'
    },
    {
      report: 'Situation report - 50',
      date: ' 10 March 2020',
      pdf: 'https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200310-sitrep-50-covid-19.pdf?sfvrsn=55e904fb_2'
    },
    // .....
  ]
]
```


### PluginManager.getTaskForceInfoUS()
*From the White House Coronavirus Task Force*
  - *What every American and community can do now to decrease the spread of the coronavirus*
  - *Recommendations for 30-Day Mitigation Strategies*

```json
[
  [
    {
      state: 'Keeping workplaces, homes, schools, or commercial establishments safe',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/workplace-school-and-home-guidance.pdf'
    },
    {
      state: 'CDC’s framework for mitigation',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/community-mitigation-strategy.pdf'
    },
    {
      state: 'Florida',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/FL_Community_Mitigation.pdf'
    },
    {
      state: 'Massachusetts',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/MA_Community_Mitigation.pdf'
    },
    {
      state: 'New Rochelle, NY',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/New-Rochelle_Community_Mitigation.pdf'
    },
    {
      state: 'Santa Clara, CA',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/Santa-Clara_Community_Mitigation.pdf'
    },
    {
      state: 'Seattle, WA',
      pdf: 'https://www.cdc.gov/coronavirus/2019-ncov/downloads/Seattle_Community_Mitigation.pdf'
    }
  ]
]
```

### PluginManager.getGlobalData();
- *Public data of each country, with updated data in real time.*
  - *The problem with this function is that the data takes a little time to display, this is due to the large amount of data that is added to [COVID-19 google spreadsheets](https://docs.google.com/spreadsheets/d/1avGWWl1J19O_Zm0NGTGy2E-fOG05i4ljRfjl87P7FiA/htmlview?ts=5e5e9222&sle=true#gid=0).*
  - *According to information it is possible that the data is moved due to the large amount of data on the page. Eventually any changes I will be aware of.*
  - *Since the data is not well parsed I leave you a table referencing the properties:*
  - | Object Properties      | 
    | ---------------------- |
    |A = Province/State      |
    |B =  date               |
    |C = Case Type           |
    |D = Cases               |
    |E = Long                |
    |F = Lat                 |
    |D = Difference          |
    |H = Last Update Date    |

```json
  {
    "53065": "Argentina",
    "A": "",
    "B": "2020-03-15",
    "C": "Confirmed",
    "D": "45",
    "E": "-63.6167",
    "F": "-38.4161",
    "G": "11",
    "H": "2020-03-16 12:08:25"
  },  
  {
    "53065": "Armenia",
    "A": "",
    "B": "2020-01-22",
    "C": "Confirmed",
    "D": "0",
    "E": "45.0382",
    "F": "40.0691",
    "G": "0",
    "H": "2020-03-16 12:08:25"
  },
```

### PluginManager.getTestsInUS()
*Reporting public health labs are 48 state public health labs (AK, AL, AR, AZ, CA, CO, CT, DE, FL, GA, HI, IA, ID, IL, IN, KS, KY, LA, MA, MD, ME, MI, MN, MO, MS, MT, NC, ND, NE, NH, NJ, NM, NV, NY, OH, OK, OR, PA, RI, SC, SD, TN, TX, VT, WA, WI, WV and WY), New York City, USAF, and 9 California counties.*
 - *Non-respiratory specimens were excluded. For state public health labs, the date represents the date of sample collection, if available, or the date tested. For CDC labs, the date represents the date specimen was received at CDC.*
 - *[Centers for Disease Control and Prevention Testing in U.S. ](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/testing-in-us.html)*

```json
[
  [
    // .....
    {
      'Date Collected': '3/10',
      'CDC Labs': '139',
      'US Public Health Labs': '2567'
    },
    {
      'Date Collected': '3/11',
      'CDC Labs': '107',
      'US Public Health Labs': '2637'
    },
    {
      'Date Collected': '3/12',
      'CDC Labs': '75‡',
      'US Public Health Labs': '2302‡'
    },
    {
      'Date Collected': '3/13',
      'CDC Labs': '0‡',
      'US Public Health Labs': '1511‡'
    },
    {
      'Date Collected': '3/14',
      'CDC Labs': '0‡',
      'US Public Health Labs': '165‡'
    },
    {
      'Date Collected': '3/15',
      'CDC Labs': '0‡',
      'US Public Health Labs': '4‡'
    }
  ]
]
```

## 💡 References
- *worldometers. 2020. Coronavirus. [online] Available at: <https://www.worldometers.info/coronavirus/> [Accessed 16 March 2020].*
- *cdc.gov. 2020. From the White House Coronavirus Task Force [online] Available at: <https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/from-the-white-house-task-force.html/>*
- *who. 2020. Coronavirus disease (COVID-2019) situation reports [online] Available at: <https://www.who.int/emergencies/diseases/novel-coronavirus-2019/situation-reports/> [Accessed 16 March 2020]*


## **:handshake: Contributing**

- Fork it!
- Create your feature branch: `git checkout -b my-new-feature`
- Commit your changes: `git commit -am 'Add some feature'`
- Push to the branch: `git push origin my-new-feature`
- Submit a pull request

---

### **:busts_in_silhouette: Credits**

- [Chris Michael](https://github.com/ChrisMichaelPerezSantiago) (Project Leader, and Developer)

---

### **:anger: Troubleshootings**

This is just a personal project created for study / demonstration purpose and to simplify my working life, it may or may
not be a good fit for your project(s).

---

### **:heart: Show your support**

Please :star: this repository if you like it or this project helped you!\
Feel free to open issues or submit pull-requests to help me improving my work.


---


### **:robot: Author**

_*Chris Michael*_

> You can follow me on
[github](https://github.com/ChrisMichaelPerezSantiago)&nbsp;&middot;&nbsp;[twitter](https://twitter.com/Chris5855M)

---

Copyright © 2020 [COVID19 API](https://github.com/ChrisMichaelPerezSantiago/covid19).
