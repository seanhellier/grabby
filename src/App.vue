<template>
  <div id="app" class="small-container">

    <employee-form />
    <h1>Employees</h1>

      <employee-table :employees="employees" />
  </div>
</template>

<script>
/* eslint-disable */

  import EmployeeTable from '@/components/EmployeeTable.vue';
  import EmployeeForm from '@/components/EmployeeForm.vue';

  export default {
    name: 'app',
    components: {
      EmployeeTable,
      EmployeeForm,
    },
   data() {
    return {
      employees: [
        {
          id: 1,
          name: 'Richard Hendricks',
          email: 'richard@piedpiper.com',
        },
        {
          id: 2,
          name: 'Bertram Gilfoyle',
          email: 'gilfoyle@piedpiper.com',
        },
        {
          id: 3,
          name: 'Dinesh Chugtai',
          email: 'dinesh@piedpiper.com',
        },
      ],
    }
  }
}

</script>

<style>
#app {
  
}
</style>
