# Crawling
국내/외 쇼핑몰 크롤링

#### *Made by cheonsol lee - Updated(2020.08.11)* ####

----------
### 1. 목적
국내 쇼핑몰 : 옥션, 다나와
국외 쇼핑몰 : 아마존, 볼(네덜란드)

해당 쇼핑몰에 대해 특정 키워드를 검색하고 각 제품의 이름, 가격, 판매자, 용량을 csv파일로 출력해주는 프로그램을 제작한다.


----------
### 2. 특징
* 옥션, 볼 : 정적크롤링
* 다나와, 아마존 : 동적크롤링

정적크롤링의 경우 beautifulSoup만으로 구현이 가능하였으나, 동적크롤링은 selenium과 beautifulSoup을 모두 사용하였다.


----------
### 3. 설치할 것

* import requests
* from bs4 import BeautifulSoup
* import pandas as pd
* import csv
* import os
* from selenium

Chrome버전에 맞는 ChromeDriver를 설치해야한다.
크롬드라이버 설치 : https://chromedriver.chromium.org/downloads


----------
### 4. 실행방법
* file_path, site_name, keyword, chromedriver_path를 사용자의 환경에 맞게 변경한다.
* 실행부의 crawling()함수를 실행하면 아래에 테이블구조를 볼 수 있으며 지정한 경로에 '쇼핑몰명_키워드명.csv'형태의 파일이 생성된다.
  * ex) Auction_hemp.csv
