- 👋 Hi, I’m @Raihan2503
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Hello My Name is Raihan Alfaridzi Kustiawan this is a first my project create a komikstore
using javascript
// Variabel Komik
let komik = ["Naruto", "One Punch Man"]
let hargaBiasa = [125000, 150000]
let hargaJual = [150000, 200000]
let penulis = ["Masashi Kishimoto", "Murata Sensei"]
let keranjang = [];
let pendapatan = 0;
let keuntungan = 0;

// membuat function tampil data
function tampilData() {
 for( let i = 0; i < komik.length; i++) {
   console.log(`${i+1}. ${komik[i]}\t Rp. ${hargaJual[i]}`)
 }
}

function BeliKomik(data, bayar) {
  for(let i = 0; i < komik.length; i++) {
    if(komik[i] == data) {
      if(bayar == hargaJual[i]) {
        keranjang.push(data)
        pendapatan += bayar;
        keuntungan += hargaJual[i] - hargaBiasa[i]
        return console.log(`Komik yang anda beli : ${komik[i]} \nHarga : Rp. ${hargaJual[i]}`);
      } else if(bayar > hargaJual[i]) {
        keranjang.push(data)
        pendapatan += hargaJual[i];
        keuntungan += hargaJual[i] - hargaBiasa[i]
        return console.log(`Komik yang anda beli : ${komik[i]} \nHarga : Rp. ${hargaJual[i]}\nKembaian : ${bayar - hargaJual[i]}`)
      }
      return "Uang anda tidak cukup!"
    }
  }
   return "Komik yang anda cari tidak ada!"
}

// Menambah data baru
function tambahData(judulKomik, hargaKomik, Penulis, hargaPasar) {
  for(let i = 0; i < komik.length; i++) {
    if(judulKomik == komik[i]) {
      return "Judul komik sudah ada!"
    }
    komik.push(judulKomik)
    hargaJual.push(hargaKomik)
    penulis.push(Penulis)
    hargaBiasa.push(hargaPasar)
    return
  }
}

// Membuat Detail Komik
function detailKomik(judulKomik) {
  for(let i = 0; i < komik.length; i++) {
    if(judulKomik == komik[i]) {
      console.log(`Detail Komik \nJudul Komik : ${komik[i]}\n Harga : Rp. ${hargaJual[i]}\n Penulis : ${penulis[i]}`);
      return
    }
  }
  return "Judul Komik tidak ada!"
}

--->
