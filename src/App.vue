

<template>
  <section class="dashboard-container">
    <!-- ========================
              Header-part-starts 
       ========================== -->
    <header class="header-container">
      <nav class="navbar navbar-expand-lg bg-transparent navbar-custom p-0">
        <div class="container-fluid flex-nowrap p-0">
          <button :class="{ 'd-none': showSidebar }" class="navbar-toggler" @click="showSidebar = !showSidebar"
            type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll"
            aria-expanded="t" aria-label="Toggle navigation">
            <img src="./assets/Svg/logo.svg" alt="">
          </button>
          <form class="">
            <img src="./assets/Svg/Vector.svg" alt="" class="position-absolute ps-4 svg-vector">
            <input class="form-control input-field" type="search" placeholder="Search Here ....">
          </form>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
            aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ms-auto">
              <li class="d-flex  justify-content-around align-items-center me-5">
                <div>
                  <button type="button" class="btn btn-none">
                    <img src="./assets/Svg/45-chat.svg" alt="">
                    <h1 class="translate-middle badge custom-badge">
                      2
                    </h1>
                  </button>
                </div>
                <div>
                  <button type="button" class="btn btn-none">
                    <img src="./assets/Svg/announcement.svg" alt="">
                    <h1 class="translate-middle badge custom-badge">
                      2
                    </h1>
                  </button>
                </div>
                <div class="px-3 py-1">
                  <img src="./assets/Svg/Setting.svg" alt="">
                </div>
              </li>
              <div class="nav-item">
                <div class="d-flex align-content-center">
                  <div class="image-admin me-4">
                  </div>
                  <div className="admin-details">
                    <h5>Madison Eve</h5>
                    <p>Admin</p>
                  </div>
                </div>
              </div>
            </ul>
          </div>
        </div>
      </nav>
      <!-- ========================
                  Main-Contents-starts
          ========================== -->
      <main class="dashboard-content">
        <h1 class="dashboard-heading">Dashboard</h1>
        <div class="row">
          <div class="col-md-3">
            <div class="card-container">
              <div class="d-flex align-items-center mt-sm-2">
                <div class="card-image">
                  <img src="./assets/Svg/Bag.svg" alt="" />
                </div>
                <div class="ms-4 card-sub-heading">
                  <h5>Projects</h5>
                  <h6>932</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="card-container">
              <div class="d-flex align-items-center mt-sm-2">
                <div class="card-image">
                  <img src="./assets/Svg/Graph.svg" alt="" />
                </div>
                <div class="ms-4 card-sub-heading">
                  <h5>Projects</h5>
                  <h6>932</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="card-container">
              <div class="d-flex align-items-center mt-sm-2">
                <div class="card-image">
                  <img src="./assets/Svg/Graph.svg" alt="" />
                </div>
                <div class="ms-4 card-sub-heading">
                  <h5>Projects</h5>
                  <h6>932</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="card-container">
              <div class="d-flex align-items-center pt-sm-2">
                <div class="card-image">
                  <img src="./assets/Svg/Investments.svg" alt="" />
                </div>
                <div class="ms-4 card-sub-heading">
                  <h5>Projects</h5>
                  <h6>932</h6>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
      <!-- ========================
                  Main-Contents-ends
          ========================== -->

    </header>
    <!-- ========================
              Header-part-ends 
       ========================== -->

    <aside class="sidebar-container d-none d-lg-block" :style="showSidebar && { display: 'block !important' }">
      <nav class="navbar-expand-lg">
        <button class="navbar-toggler dashboard-main-icon" type="button" data-bs-toggle=" collapse"
          @click="showSidebar = !showSidebar" data-bs-target="#navbarScroll" aria-controls="navbarScroll"
          :style="showSidebar && { display: 'block !important' }" aria-expanded="t" aria-label="Toggle navigation">
          <img src="./assets/Svg/logo.svg" alt="">
        </button>
        <ul class="navbar-nav logo-container" style="--bs-scroll-height: 100px;">
          <li class="nav-item d-none d-lg-inline-block dashboard-main-icon" :style="{}">
            <img src="./assets/Svg/logo.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/Home.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/1-mail.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/47-team.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/20-dollar-symbol.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/46-task.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/4-list.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/Wallet.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/25-credit-card.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/34-folder.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/2-user.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/Calendar.svg" alt="">
          </li>
          <li class="nav-item dashboard-icon">
            <img src="./assets/Svg/10-todo.svg" alt="">
          </li>
        </ul>
      </nav>
    </aside>

    <!-- ========================
                      slider-part-ends 
              ========================== -->
  </section>
</template>

<script setup>
import { ref } from "vue";
const showSidebar = ref(false)
</script>

<style scoped>

</style>
