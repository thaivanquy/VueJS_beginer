<template>
  <aside
    class="
      sidenav
      bg-white
      navbar navbar-vertical navbar-expand-xs
      border-0 border-radius-xl
      my-3
      fixed-start
      ms-4
    "
    id="sidenav-main"
  >
    <div class="sidenav-header">
      <i
        class="
          fas
          fa-times
          p-3
          cursor-pointer
          text-secondary
          opacity-5
          position-absolute
          end-0
          top-0
          d-none d-xl-none
        "
        aria-hidden="true"
        id="iconSidenav"
      ></i>
      <a class="navbar-brand m-0" href="#" target="_blank">
        <img :src="logoCtDark" class="navbar-brand-img h-100" alt="main_logo" />
        <span class="ms-1 font-weight-bold">Argon Dashboard 2</span>
      </a>
    </div>
    <hr class="horizontal dark mt-0" />
    <div class="collapse navbar-collapse w-auto" id="sidenav-collapse-main">
      <ul class="navbar-nav">
        <li class="nav-item">
          <router-link class="nav-link active" :to="{ name: 'dashboard'}">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-tv-2 text-primary text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">Dashboard</span>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" :to="{ name: 'users'}">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i
                class="ni ni-calendar-grid-58 text-warning text-sm opacity-10"
              ></i>
            </div>
            <span class="nav-link-text ms-1">Users</span>
          </router-link>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-credit-card text-success text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">Billing</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-app text-info text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">Virtual Reality</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-world-2 text-danger text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">RTL</span>
          </a>
        </li>
        <li class="nav-item mt-3">
          <h6
            class="
              ps-4
              ms-2
              text-uppercase text-xs
              font-weight-bolder
              opacity-6
            "
          >
            Account pages
          </h6>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-single-02 text-dark text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">Profile</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i
                class="ni ni-single-copy-04 text-warning text-sm opacity-10"
              ></i>
            </div>
            <span class="nav-link-text ms-1">Sign In</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <div
              class="
                icon icon-shape icon-sm
                border-radius-md
                text-center
                me-2
                d-flex
                align-items-center
                justify-content-center
              "
            >
              <i class="ni ni-collection text-info text-sm opacity-10"></i>
            </div>
            <span class="nav-link-text ms-1">Sign Up</span>
          </a>
        </li>
      </ul>
    </div>
    <div class="sidenav-footer mx-3">
      <div class="card card-plain shadow-none" id="sidenavCard">
        <img class="w-50 mx-auto" :src="iconDoc" alt="sidebar_illustration" />
        <div class="card-body text-center p-3 w-100 pt-0">
          <div class="docs-info">
            <h6 class="mb-0">Need help?</h6>
            <p class="text-xs font-weight-bold mb-0">Please check our docs</p>
          </div>
        </div>
      </div>
      <a href="#" target="_blank" class="btn btn-dark btn-sm w-100 mb-3"
        >Documentation</a
      >
      <a class="btn btn-primary btn-sm mb-0 w-100" href="#" type="button"
        >Upgrade to pro</a
      >
    </div>
  </aside>
</template>
<script>
import logoCtDark from "@/assets/img/logo-ct-dark.png";
import iconDoc from "@/assets/img/illustrations/icon-documentation.svg";

export default {
  name: "ComSideNav",
  data() {
    return {
      logoCtDark,
      iconDoc,
    };
  },
};
</script>
