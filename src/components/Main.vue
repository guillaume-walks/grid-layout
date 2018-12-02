  <template>
      <div class="main">
        <h2>content</h2>
        <div class="sub-content">
          <div class="item">item element </div>
          <div class="item">item element </div>
          <div class="item">item element </div>
          <div class="item">item element </div>
          <div class="item">item element </div>
        </div>
      </div>
  </template>
  
  <script>
  export default {
    name: 'Main'
  }
  </script>
  <style>
  .main{
    grid-column: 2/3;
  }
  
  .sub-content{
    display: grid;
  }

  .sub-content > * {
    border: 1px dashed lightgray;
  }
  </style>
  
  