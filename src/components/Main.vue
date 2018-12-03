  <template>
  <div class="main">
    <h2>content</h2>
    <div class="sub-content">
      <div class="item1">item element 1</div>
      <div class="item2">item element 2</div>
      <div class="item3">item element 3</div>
      <div class="item4">item element 4</div>
      <div class="item5">item element 5</div>
      <div class="item6">item element 6</div>
    </div>
  </div>
</template>
  
  <script>
export default {
  name: "Main"
};
</script>
  <style>
.main {
  grid-column: 2/3;
  height: 100%;
  align-content: center;
}

.sub-content {
  display: grid;
  /* height: 700px; */
  align-content: center;
  grid-gap: 10px;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr 1fr;
  background: lightblue;
  padding: 10px;
}
.item1 {
  grid-area: 1 / 1 / 3 / 4;
}
.item2 {
  grid-area: 2 / 4 / 3 / 6;
}
.item3 {
  grid-area: 3 / 3 / 4 / 5;
}
.item4 {
  grid-area: 4 / 2 / 5 / 6;
}
.item5 {
  grid-area: 5 / 1 / 6 / 3;
}
.item6 {
  grid-area: 5 / 4 / 6 / 7;
}
@media screen and (max-width: 750px) {
  .item1 {
    grid-area: 1 / 1 / 2 / 2;
  }
  .item2 {
    grid-area: 2 / 1 / 3 / 2;
  }
  .item3 {
    grid-area: 3 / 1 / 4 / 2;
  }
  .item4 {
    grid-area: 1 / 2 / 2 / 7;
  }
  .item5 {
    grid-area: 2 / 2 / 2 / 7;
  }
  .item6 {
    grid-area: 3 / 2 / 3 / 7;
  }
}
.sub-content > * {
  border: 1px dashed rgb(143, 143, 143);
  padding: 10px;
  background: rgb(206, 243, 255);
}
</style>
  
  