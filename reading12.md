[README.MD](README.md)   
[EJS Partial](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)  


**EJS Partials**  

- make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.  
- In this reading it mentioned how the footer in their example appeared twice, which is a good thing. Along with the NAV bar.  
- They created two different EJS files so that the material can be referenced as it appears multiple times.  
- In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters.  
- The <%- %> tags allow us to output the un-escaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…  
- Now the partials can be referenced from their folders and kept clean in their layout.  