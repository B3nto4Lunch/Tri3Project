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

<table>
  <thead>
    <tr>
      <th>Lesson</th>
      <th>Topic</th>
      <th>Game Element</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Samit</td>
      <td>Iteration, Lists, Random Values, Simulations</td>
      <td>Random generation of game elements (e.g. enemies, obstacles)</td>
    </tr>
    <tr>
      <td>Martin</td>
      <td>Algorithms, Calling and Developing Procedures, Algorithmic Efficiency, Undecidable Problems</td>
      <td>Implementation of game logic using algorithms and procedures</td>
    </tr>
    <tr>
      <td>Akshat</td>
      <td>Conditionals, Nested Conditionals, Binary Search (Selection)</td>
      <td>Conditionals and selection of game elements based on player input</td>
    </tr>
    <tr>
      <td>Ederick</td>
      <td>Variables and Assignments, Data Abstraction, Mathematical Expressions, Strings, and Boolean Expressions (Review Topics)</td>
      <td>Use of variables and expressions to track game state and handle player input</td>
    </tr>
    <tr>
      <td>Joselyn</td>
      <td>Using SQLite libraries to create a database with simulation data (Database)</td>
      <td>Implementation of leaderboard system using SQLite database</td>
    </tr>
  </tbody>
</table>



