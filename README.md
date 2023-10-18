<p align="center"><img width="500" src="./assets/slash.png"></p>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/704785726.svg)](https://zenodo.org/badge/latestdoi/704785726)
[![GitHub issues](https://img.shields.io/github/issues/ameghana/CSC510-FALL23-P27-Project2)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/ameghana/CSC510-FALL23-P27-Project2)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/issues?q=is%3Aissue+is%3Aclosed)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/ameghana/CSC510-FALL23-P27-Project2)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/pulls?q=is%3Aopen+is%3Apr)
[![Npm package version](https://badgen.net/npm/v/express)](https://npmjs.com/package/express)
[![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.63.0-009688.svg?style=flat&logo=FastAPI&logoColor=white)](https://fastapi.tiangolo.com)
[![GitHub contributors](https://img.shields.io/github/contributors/ameghana/CSC510-FALL23-P27-Project2)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/graphs/contributors)
![GitHub all releases](https://img.shields.io/github/downloads/ameghana/CSC510-FALL23-P27-Project2/total)
[![GitHub Discussions](https://img.shields.io/github/discussions/ameghana/CSC510-FALL23-P27-Project2)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/discussions)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
![Discord](https://img.shields.io/discord/1161405668079698112)
![GitHub forks](https://img.shields.io/github/forks/ameghana/CSC510-FALL23-P27-Project2)
[![codecov](https://codecov.io/gh/NCSU-Group7-SE2021/slash/branch/main/graph/badge.svg?token=E9TCZQ6NGF)](https://codecov.io/gh/NCSU-Group7-SE2021/slash)

Do you love shopping? Are you in search of some good deals while shopping online?! Slash is here to help you look for the best deals!

Slash is an open-source web framework that makes use of FastAPI to scrape the best deals from various e-commerce websites such as eBay, Amazon, BestBuy, Costco, Target, and Walmart. Slash makes it easy for users to filter,organise and download search results.It also provides visualisation in the form of charts and graphs.

- **Fast**: With slash, you can save over 50% of your time by comparing deals across websites within seconds
- **Easy**: Slash introduces easy to use public APIs to filter, sort and search through the search results
- **Powerful**: Produces JSON responses that can be easily customised to bring about the desired output

---

## :rocket: Improvements over Phase-II

We have added a lot of new features to slash in our Phase-III.

1. A web interface for users to interact with the application in a more native way.
2. Charts and graphs for better visualization of the results.
3. Analysis for price prediction of products.
4. Analysis for variety count of products per e-commerce store.

---

<p align="center">
  <a href="#movie_camera-checkout-our-video">Checkout our video</a>
  ::
  <a href="#rocket-installation">Installation</a>
  ::
  <a href="#computer-technology-used">Technology Used</a>
  ::
  <a href="#bulb-use-case">Use Case</a>
  ::
  <a href="#file_cabinet-api">API</a>
  ::
  <a href="#page_facing_up-why">Why</a>
  ::
  <a href="#golf-future-roadmap">Future Roadmap</a>
  ::
  <a href="#sparkles-contributors">Contributors</a>
  ::
  <a href="#email-support">Support</a>

</p>

---

## :movie_camera: Checkout our video

<p align="center"><img width="700" src="./assets/slash-phase3.gif"></p>

---

## :rocket: Installation

1. Clone the Github repository to a desired location on your computer. You will need [git](https://git-scm.com/) to be preinstalled on your machine. Once the repository is cloned, you will then `cd` into the local repository.

```
git clone https://github.com/secheaper/slash.git
cd slash
```

2. This project uses Python 3 for the backend and React framework for the frontend.

For the backend setup ensure that [Python](https://www.python.org/downloads/) and [Pip](https://pip.pypa.io/en/stable/installation/) are preinstalled. All the python requirements of the project are listed in the `requirements.txt` file. Use pip to install all of those.

```
pip3 install -r requirements.txt
```

For the frontend setup ensure that [Node](https://nodejs.org/en/) is preinstalled. All the node requirements are listed in `client/package.json` file. Use npm to install all of those.

```
cd client
npm install
```

4. Once all the requirements are installed, you will have to `cd` into the `src` folder. Once in the `src` folder, use the python command to run the `main.py` file.

```
cd src

For Mac
python3 main.py

For Windows
python main.py
```

5. Once the backend is up and running, you will have to `cd` into the `client` folder. Once in the `client` folder, use the node command to start the webserver.

```
cd client
npm run start
```

## :computer: Technology Used

- FastAPI : https://fastapi.tiangolo.com
- ASGI Server - Uvicorn : https://www.uvicorn.org
- Docker : https://www.docker.com
- Azure : https://azure.microsoft.com/en-us/

## :bulb: Use Case

- **_Students_**: Students coming to university are generally on a budget and time constraint and generally spend hours wasting time to search for products on Websites. Slash is the perfect tool for these students that slashes all the unnecessary details on a website and helps them get prices for a product across multiple websites.Make the most of this tool in the upcoming Black Friday Sale.
- **_Data Analysts_**: Finding data for any project is one of the most tedious job for a data analyst, and the datasets found might not be the most recent one. Using slash, they can create their own dataset in real time and format it as per their needs so that they can focus on what is actually inportant.

## :file_cabinet: API

## Documentation

Documentation can be accessed anytime via the below link.

     `https://slash-app-staging.azurewebsites.net/`

## Search Items Api

Wrapper API to fetch slash scrape results. This API provides a one step solution to access scrape results from all our integrated websites.

    https://slash-app-staging.azurewebsites.net/{site}/{item_name}

**Required parameters:**

- **site**: _az_ for amazon; _wm_ for walmart; _eb_ for ebay; _cc_ for costco; _tg_ for target and _bb_ for bustbuy. Alternatively '_all_' in site can be used to get results for all sites.

- **item_name**: items to be searched by slash web api; _examples below_

`https://slash-app-staging.azurewebsites.net/az/toys`

`https://slash-app-staging.azurewebsites.net/all/dell`

**Optional parameters**

- **relevant**: string relevance: items will be ordered by relevance. Not supported currently.
- **order_by_col**: string column_name: items will be ordered by the column name. Currently only the 'price' column ordering is supported.
- **reverse**: boolean val: items will be displayed in the same or the opposite order based on the value of this parameter.
- **listLengthInd**: integer len(default value is 10): sets the upper limit on the number of entries that will be displayed
- **export**: boolean val(default value is false): items can be exported in a csv file;; _examples below_

`https://slash-app-staging.azurewebsites.net/all/dell?export=false&listLengthInd=5&order_by_col=price&reverse=false`

## :page_facing_up: Why

- In a market where we are spoilt for choices, we often look for the best deals.
- The ubiquity of internet access has leveled the retail playing field, making it easy for individuals and businesses to sell products without geographic limitation. In 2020, U.S. e-commerce sales, receiving a boost due to the COVID-19 pandemic, grew 44% and represented more than 21% of total retail sales, according to e-commerce information source Internet Retailer.
- The growth of e-commerce has not only changed the way customers shop, but also their expectations of how brands approach customer service, personalize communications, and provide customers choices.
- E-commerce market has prompted cut throat competition amongst dealers, which is discernable through the price patterns for products of major market players. Price cuts are somewhat of a norm now and getting the best deal for your money can sometimes be a hassle (even while online shopping).
- This is what Slash aims to reduce by giving you an easy to use, all in one place solution for finding the best deals for your products that major market dealers have to offer!
- Slash in its current form is for students who wish to get the best deals out of every e-commerce site and can be used by anyone who is willing to develop an application that consumes these web APIs.
- Future scope includes anything from a web application with a frontend or any Android or IOS application that utilises these Web APIs at their backend. Anyone can build their own custom application on top of these web APIs.

## :golf: Future Roadmap

- Host website on a public server so customers can use it
- Add login feature to store user history to provide features like bookmarking, price drop alerts and many more.
- Our API can be used by end users such as developers who are tech-savvy individuals looking to get a one stop solution for web scraping ecommerce websites such as Amazon, Target, Ebay,etc along with API access to multiple ecommerce websites. It'll be available directly for access to people without having to dive deep into the code.
- An iOS or Android application.
- Add reviews to the products

# Team Members

## Phase 2 Team Members

- [Meghana Chowdary Ainampudi](https://github.com/ameghana)
- [Sai Abhigna Tummala](https://github.com/abhigna98)
- [Sravya Karanam](https://github.com/SreeKaranam)
- [Sucharitha Nadendla](https://github.com/Nsucharitha)

## :email: Support

For any queries and help, please reach out to us at: SEslash007@gmail.com
