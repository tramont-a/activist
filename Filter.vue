<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1 class="title">{{ msg }}</h1>
    <div class="btn-tabs">
      <button>Active</button>
      <button>New</button>
      <button>Private</button>
    </div>
    <input type="text" placeholder="Search to filter"/>
    <h3>
      Popular tags
    </h3>
    <div class="btn-tag">
      <button>Tag</button>
      <button>Tag</button>
      <button>Tag</button>
      <button>Tag</button>
      <button>Tag</button>
    </div>
    <table>
      <tr>
        <th>Cause</th>
        <th>Synopsis</th>
        <th>More Info</th>
      </tr>
      <tr>
        <td>Cause 1</td>
        <td>Summary</td>
        <td>Click here for their website</td>
      </tr>
      <tr>
        <td>Cause 2</td>
        <td>Summary</td>
        <td>Click here for their website</td>
      </tr>
      <tr>
        <td>Cause 3</td>
        <td>Summary</td>
        <td>Click here for their website</td>
      </tr>
    </table>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.2rem;
  position: fixed;
  top: 3px;
  left: 10px;
}

.btn-tabs {
  display: inline;
  float: right;
  position: absolute;
  top: 20px;
  right: 10px;
}

.btn-tag {
  display: inline;
  float: left;
  position: absolute;
  top: 120px;
  left: 2vw;
}

button {
  padding: 8px 20px;
  background-color: #c8c8c8;
  border: transparent;
}

button:hover {
  background-color: #f4a454;
  color: white;
  cursor: pointer;
}

button:focus {
  background-color: #f4a454;
  color: white;
}

input[type=text] {
  background-color: #f0f0eb;
  box-shadow: 2px 3px #dfe0df;
  border-radius: 4px;
  border: none;
  font-size: 17px;
  width:97vw;
  position: absolute;
  top: 70px;
  left: 1.5vw;
}

table {
  width: 97vw;
  position: absolute;
  top: 165px;
  left: 1.5vw;
}

td, th {
  border: 1px solid #dfe0df;
  text-align: left;
  padding: 8px;
}

th {
  font-weight: bold;
  color: white;
  background-color: #36322e;
}

tr:hover {
  background-color:#f4a454;
  color: white;
}

tr:nth-child(even) {
  background-color: #cccccc;
}

tr:nth-child(even):hover {
  background-color:#f4a454;
  color: white;
}

h3 {
  font-size: 0.8rem;
}

.greetings h1 {
  text-align: left;
}

.greetings h3 {
  text-align: left;
  position: absolute;
  top: 100px;
  left: 2vw;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
