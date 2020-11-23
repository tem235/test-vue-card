<template>
  <div class="card">
    <div class="card-header">
      <h3 class="card-header__title">Traffic Runners, LLC</h3>
      <h5 class="card-header__subtitle">Software company</h5>
    </div>
    <div class="card-btn-group">
      <button class="btn active"><img src="@/assets/list.svg" alt="">Standard</button>
      <button class="btn"><img src="@/assets/calendar.svg" alt="">Event</button>
      <button class="btn" disabled><img src="@/assets/bell.svg" alt="">Alert</button>
    </div>
    <div class="card-from">
      <label class="card-from__label" for="example">Link to the button </label>
      <input class="card-from__input" id="example" type="text">
    </div>
    <div class="card-text">
      <p>You can use any link, but it’s length should not exceed
        200 characters</p>
    </div>
    <button class="btn btn--primary">Continue</button>
  </div>
</template>

<script>
export default {
  name: "Card"
}
</script>

<style scoped>
.card {
  width: 512px;
  height: 480px;
  padding: 36px 25px 71px 32px;
  border-radius: 4px;
  box-shadow: 0 8px 8px 0 rgba(119, 131, 143, 0.16);
  background-color: #ffffff;
  text-align: left;
  box-sizing: border-box;
}

.card-header {
  margin-bottom: 26px;
}

.card-header__title {
  font-size: 24px;
  font-weight: bold;
  margin: 0 0 5px;
}

.card-header__subtitle {
  font-size: 18px;
  font-weight: 600;
  margin: 0;
  color: #828e9a;
}

.card-btn-group {
  display: flex;
  height: 40px;
  margin-bottom: 33px;
}

.card-btn-group button {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  border: none;
  border-radius: 0;
  width: 150px;
  background-color: #e7eaf3;
  font-size: 16px;
  font-weight: 400;
  color: #77838f;
  margin-right: 1px;
}

.card-btn-group button img {
  margin-right: 8px;
}

.card-btn-group button:hover {
  background-color: #377dff;
  color: #fff;
}

.card-btn-group button.active {
  background-color: #377dff;
  color: #fff;
}

.card-btn-group button:first-child {
  border-radius: 24px 0 0 24px;
}

.card-btn-group button:last-child {
  border-radius: 0 24px 24px 0;
}


.card-from__label {
  display: inline-block;
  color: #77838f;
  font-size: 18px;
  font-weight: 400;
  margin-bottom: 5px;
}

.card-from__input {
  box-sizing: border-box;
  width: 100%;
  height: 48px;
  border-radius: 24px;
  padding-left: 20px;
  border: solid 1px rgba(119, 131, 143, 0.56);
}

.card-from__input:focus {
  outline: none;
}

.card-text {
  width: 90%;
  font-size: 16px;
  line-height: 1.5;
  margin-bottom: 17px;
}


.btn {
  padding: 0;
  border-radius: 28px;
  border: none;
  color: #fff;
  font-size: 18px;
  font-weight: 400;
  transition: .3s;
}

.btn:hover {
  cursor: pointer;
}

.btn:focus {
  outline: none;
}

.btn:disabled {
  cursor: not-allowed;
  opacity: .7;
  background: #ccc;
}

.btn:disabled:hover {
  cursor: not-allowed;
  opacity: .7;
  background: #ccc;
  color: #77838f;
}

.btn--primary {
  width: 208px;
  height: 48px;
  background-color: #377dff;
}

.btn--primary:hover {
  background-color: #0f60f7;
}
</style>