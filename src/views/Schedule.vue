<template>
  <div class="about">
    <h1 style="font-family: 'Bebas Neue', cursive;">Jadwal Pelatihan</h1>

    <table class="highlight centered" style="margin-bottom:200px;margin-left:auto;margin-right:auto;width:70%;">
      <thead>
        <tr>
          <th>Waktu</th>
          <th>Materi</th>
          <th>Narasumber</th>
        </tr>
      </thead>

      <tbody>
        <tr>
          <td>{{ getDate(0) }}</td>
          <td>Manajemen Logistik</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(1) }}</td>
          <td>Standar Prosedur Operasional (SOP) Logistik	</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(2) }}</td>
          <td>Manajemen Rantai Pasok (Analisa dan Solusi)</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(3) }}</td>
          <td>Manajemen Pergudangan</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(4) }}</td>
          <td>Manajemen Material Handling</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(5) }}</td>
          <td>Manajemen Persediaan</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(6) }}</td>
          <td>Manajemen Transportasi & Distribusi</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(7) }}</td>
          <td>Keselamatan dan Kesehatan Kerja</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(8) }}</td>
          <td>Sistem Informasi Logistik</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(9) }}</td>
          <td>Manajemen Pengadaan</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(10) }}</td>
          <td>Manajemen Pelayanan Pelanggan</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(11) }}</td>
          <td>Manajemen Komunikasi</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(12) }}</td>
          <td>Manajemen Personel</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(13) }}</td>
          <td>Manajemen Finansial</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(14) }}</td>
          <td>Manajemen Ritel</td>
          <td>Tbd</td>
        </tr>
        <tr>
          <td>{{ getDate(15) }}</td>
          <td>Manajemen Freight Forwarding</td>
          <td>Tbd</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "Schedule",
  data: function () {
    return {};
  },
  methods: {
    getDate: function (week) {
      let result = new Date();
      result.setMonth(0);
      result.setDate(22 + 7 * week);
      let months = (months = [
        "Januari",
        "Februari",
        "Maret",
        "April",
        "Mei",
        "Juni",
        "Juli",
        "Agustus",
        "September",
        "Oktober",
        "November",
        "Desember",
      ]);
      let formatResult = `Jumat, ${result.getDate()} ${
        months[result.getMonth()]
      } ${result.getFullYear()}`;
      return formatResult;
    },
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');
</style>