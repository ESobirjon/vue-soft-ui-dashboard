<template>
  <div class="card mb-4">
    <div class="card-header pb-0">
      <!--      <h6>{{header}}</h6>-->
    </div>
    <div class="card-body px-0 pt-0 pb-2">
      <div class="table-responsive p-0">
        <table class="table align-items-center mb-0">
          <thead>
          <tr>
            <th class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"></th>
            <th
                class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Id
            </th>
            <th
                class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
            >
              Yuk xati raqami
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Sana
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Forma
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Qiymati
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              QQS
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Dollar qiymati
            </th>
            <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
            >
              Yaratilgan sana
            </th>
            <th class="text-secondary opacity-7"></th>
          </tr>
          </thead>
          <tbody>
          <tr>
            <td class="text-center cursor-pointer">
              <img src="@/assets/img/excel1.png" style="width: 30px; height: 35px;" alt="excel"/>
            </td>
            <td>
              <div class="d-flex px-3 py-1">
                <p class="text-xs font-weight-bold mb-0">Id</p>
              </div>
            </td>
            <td>
              <p class="text-xs font-weight-bold mb-0">Yuk xati raqami</p>
            </td>
            <td class="align-middle text-center text-sm">
              <soft-badge color="success" variant="gradient" size="sm"
              >01.02.2023
              </soft-badge
              >
            </td>
            <td class="align-middle text-center">
              <p class="text-xs font-weight-bold mb-0">Forma nomi</p>
            </td>
            <td class="align-middle text-center">
              <p class="text-xs font-weight-bold mb-0">Qiymati</p>
            </td>
            <td class="align-middle text-center">
              <p class="text-xs font-weight-bold mb-0">QQS qiymati</p>
            </td>
            <td class="align-middle text-center">
              <p class="text-xs font-weight-bold mb-0">Dollar qiymati</p>
            </td>
            <td class="align-middle text-center">
              <p class="text-xs font-weight-bold mb-0">Yaratilgan sana</p>
            </td>
            <td class="align-middle cursor-pointer">
              <img src="@/assets/img/delete1.png" style="width: 40px; height: 40px;" alt="delete">
            </td>
          </tr>
          </tbody>
        </table>
      </div>
    </div>


    <!-- PAGINATION  -->
    <div class="row justify-space-between">
      <div class="col-lg-4 mx-auto">
        <ul class="pagination pagination-primary m-4">
          <li class="page-item">
            <a class="page-link" href="" aria-label="Previous">
              <span aria-hidden="true"><i class="fa fa-angle-double-left" aria-hidden="true"></i></span>
            </a>
          </li>
          <li class="page-item active">
            <a class="page-link" style="background: #69f542" href="javascript:;">1</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="javascript:;">2</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="javascript:;">3</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="javascript:;">4</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="javascript:;">5</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="javascript:;" aria-label="Next">
              <span aria-hidden="true"><i class="fa fa-angle-double-right" aria-hidden="true"></i></span>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import SoftBadge from "@/components/SoftBadge.vue";
import img1 from "../../assets/img/team-2.jpg";
import img5 from "../../assets/img/team-2.jpg";
import img2 from "../../assets/img/team-3.jpg";
import img4 from "../../assets/img/team-3.jpg";
import img3 from "../../assets/img/team-4.jpg";
import img6 from "../../assets/img/team-4.jpg";

export default {
  name: "authors-table",
  props: {
    header: {
      type: String,
      default: () => ''
    }
  },
  data() {
    return {
      img1,
      img2,
      img3,
      img4,
      img5,
      img6,
    };
  },
  components: {
    SoftBadge,
  },
};
</script>
