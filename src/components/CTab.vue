<template>
  <div class="ctab">
    <ul class="nav nav-tabs ctab-tabs" id="myTab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home-tab-pane" type="button" role="tab" aria-controls="home-tab-pane" aria-selected="true">По номеру</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#profile-tab-pane" type="button" role="tab" aria-controls="profile-tab-pane" aria-selected="false">По шансу</button>
      </li>
    </ul>
    <div class="tab-content ctab-content" id="myTabContent">
      <div class="tab-pane fade show active" id="home-tab-pane" role="tabpanel" aria-labelledby="home-tab" tabindex="0">
        <div class="ctab-search">
          <input type="number" placeholder="Введите номер шанса">
          <button>Поиск</button>
        </div>
      </div>
      <div class="tab-pane fade" id="profile-tab-pane" role="tabpanel" aria-labelledby="profile-tab" tabindex="0">...</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .ctab{
    max-width: 650px;
    margin: 0 auto;
    &-tabs{
      width: 320px;
      margin: 0 auto;
      border-radius: 10px;
      border: 1px solid rgba(255, 255, 255, 0.50);
      background: rgba(217, 217, 217, 0.10);
      padding: 4px;
      .nav-item{
        width: 50%;
        .nav-link{
          width: 100%;
          font-size: 10px;
          color: #fff;
          font-weight: 700;
          border: 0;
          &:hover{
            border: 0;
          }
        }
        .nav-link.active{
          background: #FCFE5D;
          color: #363845;
          border-radius: 6px;
        }
      }
    }
    &-search{
      position: relative;
      input{
        border-radius: 12px;
        background: #ECF1F7;
        height: 50px;
        line-height: 50px;
        width: 100%;
        padding: 0 20px;
        border: 0;
        font-weight: 700;
        color: #000;
        &:focus{
          outline: 0;
          border: 0;
        }
      }
      button{
        position: absolute;
        top: 5px;
        right: 4px;
        height: 40px;
        line-height: 40px;
        border-radius: 10px;
        background: var(--Blue_color, #0073FF);
        box-shadow: 0px 5px 10px 0px rgba(255, 255, 255, 0.25) inset;
        border: 0;
        padding: 0 75px;
        color: #fff;
        font-size: 20px;
        font-weight: 700;
      }
    }
    &-content{
      padding-top: 40px;
    }
  }
</style>