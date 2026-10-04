# Assignment 3. Responsive Web Design (Media Queries + Bootstrap Grid)

Name: Gulim Zhumabay

Group: SE-2539

## Overview

This project is a responsive website for Coffee Lake, a cafe inside our university. The goal was to practice making pages that adjust to different screen sizes using CSS media queries and the Bootstrap 12-column grid. All parts are placed in one page with my own styles in style.css. I used three screen sizes: mobile (under 576px), tablet (576px - 992px) and desktop (993px and up).

## Task 0. Responsive Typography

Created a page with a heading and a paragraph about the cafe. With media queries the font size changes depending on the screen width. I wrote the styles for mobile first and then added two min-width media queries (576px and 993px) that override them on bigger screens.

![Task 0](screenshots/task0.png)

## Task 1. Responsive Layout with Media Queries

Created the "Why Coffee Lake?" section with three boxes (Fresh Coffee, In your university, Student Prices), using only CSS media queries and no Bootstrap classes. The container is a flex container with flex-wrap: wrap. Each box is 100% wide on mobile, so they are stacked, 50% wide on tablet, so two boxes are in a row and the third goes below, and 33.333% wide on desktop, so all three are side by side. I used box-sizing: border-box so the padding and border do not make the boxes wider than the set width.

![Task 1](screenshots/task1_desktop.png)

## Task 2. Bootstrap Responsive Columns

Built the "Special Offers" section with three columns using the Bootstrap 12-column grid. Each column has the classes col-12 col-md-6 col-lg-4. On mobile each column takes all 12 parts, so they are stacked. On tablet each takes 6 parts, so there are two columns in the first row and one in the second. On desktop each takes 4 parts, so there are three equal columns in one row. Inside every column there is a title and a list with the offer details.

![Task 2](screenshots/task2.png)

## Task 3. Bootstrap Navigation Bar

Created navigation bar with Bootstrap components. The logo of Coffee Lake is on the left and the links (Home, Menu, About, Contact) are on the right, pushed to the right side with ms-auto. The navbar uses navbar-expand-lg, so on screens wider than 992px the links are in one row, and on smaller screens they collapse into a hamburger button that opens and closes the menu on click. I also made the navbar stay at the top of the screen while scrolling with position: sticky.

![Task 3p](screenshots/task3.png)

## Task 4. Responsive Cafe Page

Built the main page of the cafe using both media queries and the Bootstrap grid. The header is the Bootstrap navbar from Task 3. The main section is divided into two parts: on the left side there are the menu cards (a col-lg-8 column with a nested row, where each card is col-12 col-md-6), and on the right side there is a sidebar (col-lg-4) with information about the cafe, opening hours and contact details (phone, Instagram, Telegram and email). On screens smaller than 992px the sidebar goes below the cards. The footer is at the bottom of the page. I also wrote custom media queries that change font sizes, paddings, photo widths and visibility of some text for mobile, tablet and desktop.

![Task 4.1](screenshots/task4.1.png)

![Task 4.2](screenshots/task4.2.png)

![Task 4.3](screenshots/task4.3.png)

## Work Process Summary

Media queries and Bootstrap were new for me, so I started with the simplest task, the responsive typography. Then I made the three boxes with flexbox and flex-wrap, and changed their width in the media queries. After that I added Bootstrap through CDN and made the same three-column behaviour with col-12 col-md-6 col-lg-4. For the navbar I used the Bootstrap component and learned how the hamburger button is connected with the menu by data-bs-toggle and data-bs-target. In the last task I combined everything: the navbar, the grid with a nested row for cards, the sidebar, the footer and my own media queries. The hardest parts for me were understanding the Bootstrap breakpoints and fixing the box widths with box-sizing: border-box. I checked every part in the browser on mobile, tablet and desktop sizes.