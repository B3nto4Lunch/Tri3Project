<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Goals</title>
    <link rel="stylesheet" href="table.css">
    <link rel="oogabooga">
</head>
<body>
  <main class = "table"> 
      <section class="table_header">
        <h1>Goals</h1>
        <table id = "table">
      <!-- </section> -->
      <section class="table_body">
        <table>
          <thead>
          <tbody id="body">
            <tr>
              <!-- <th> id </th> -->
              <th> User </th>
              <th> Object </th>
              <th> Purpose </th>
            <tr>
            <tbody>
            </tbody>
        <!-- </table> -->


<form action="javascript:createGoal()">
    <p><label>
        User:
        <input type="text"  id="goal" required>
    </label></p>
    <p><label>
        Object:
        <input type="text"  id="diff" required>
    </label></p>
     <p><label>
        Purpose:
        <input type="text"  id="time" required>
    </label></p>
      <p>
        <button>Create</button>
    </p>
</form>

