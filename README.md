# ui5\_dynamic\_load

> Test loading ui5 asynchronously by dynamically inserting the bootstrap script into the document while showing a spinner.

This app show an example of dynamically inserting the UI5 boostrap script for an asynchronous load. The page load time is far quicker than when using the standard UI5 bootstrap script in the document head. However, this page load time is just till your spinner or splash screen is displayed. Its not the time take till the UI5 views are rendered adn teh app is ready to use!

When compared based on 'UI5 views rendered to the user" then this method is slightly slower than the standard bootstrap. The benefit is that you can display html; a spinner or a splash screen to the user while UI5 loads. If you have slow load times its much better to give the user some intermediate feedback.

NOTE: Script.onload does not work properly on IE9 or Chrome 26. It is used to detect when the UI5 script has executed.

Page load times - a comparison: https://docs.google.com/spreadsheet/ccc?key=0AophLm-khFuodGJTNV9MQ0t2c05fU1phdGh3LVVJTWc&usp=sharing
