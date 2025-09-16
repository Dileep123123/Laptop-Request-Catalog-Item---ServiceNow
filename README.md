# Laptop-Request-Catalog-Item---ServiceNow
Overview

This project introduces a Service Catalog Item in ServiceNow that allows employees to request laptops through a streamlined, user-friendly, and dynamic interface.
It replaces outdated manual processes with a modern automated solution that improves accuracy, transparency, and user experience.

Features

Dynamic form behavior using Catalog UI Policies
Reset form functionality using a client-side UI Action
Clear, guided form instructions for users
Exportable Update Set for easy deployment to other ServiceNow instances
Fully tested in a separate instance to ensure smooth deployment

Variables Included

Laptop Model
Justification
Additional Accessories (checkbox/dropdown)
Accessories Details (conditionally displayed)

Dynamic Form Behavior

Implemented using Catalog UI Policies:
Show/Hide Accessories Details field based on Additional Accessories selection
Set Accessories Details as mandatory if Additional Accessories is selected

Reset Form Functionality

A client-side UI Action is included to allow users to reset the form.
UI Action Details:

Table: sc_cart
Action Name: Reset Form
Order: 100
Client: Checked

Script:

function resetForm() {
  g_form.clearForm(); // Clears all fields in the form
  alert("The form has been reset.");
}

