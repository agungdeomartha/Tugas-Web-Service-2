# Tugas-Web-Service-2

Nama  : Mohammad Agung Deomartha
NPM   : 1154032
Kelas : DIV TI 2B

<!DOCTYPE logbarang SYSTEM "logbarang.dtd">
Syntax penghubung barang.xml dan dtd logbarang

<?xml encoding="UTF-8"?>
<!ELEMENT logbarang (barang)+>
<!ATTLIST logbarang
    xmlns CDATA #FIXED ''>
<!ELEMENT barang (kode,satuan,harga?,asal,tujuan)>
<!ATTLIST barang
    xmlns CDATA #FIXED ''>
<!ELEMENT kode (#PCDATA)>
<!ATTLIST kode
    xmlns CDATA #FIXED ''>
<!ELEMENT satuan (#PCDATA)>
<!ATTLIST satuan
    xmlns CDATA #FIXED ''>
<!ELEMENT harga (#PCDATA)>
<!ATTLIST harga
    cur CDATA #IMPLIED ''>
<!ELEMENT asal (pt,kodewil)>
<!ATTLIST asal
    xmlns CDATA #FIXED ''>
<!ELEMENT tujuan (pt,kodewil)>
<!ATTLIST tujuan
    xmlns CDATA #FIXED ''>
<!ELEMENT pt (#PCDATA)>
<!ATTLIST pt
    xmlns CDATA #FIXED ''>
<!ELEMENT kodewil (#PCDATA)>
<!ATTLIST kodewil
    xmlns CDATA #FIXED ''>
    
 Sintak diatas menunjukan bahwa dtd dengan logbarang sudah terhubung dengan xmlnya.

<logbarang>

Element logbarang dari xml dengan nama barang.

<barang>
		<kode>M1112</kode>
		<satuan>pc</satuan>
		<harga cur="nmtoken">5000</harga>
	<asal>
		<pt>ladyrock</pt>
		<kodewil>10</kodewil>
	</asal>
<tujuan>
		<pt>union</pt>
		<kodewil>1001</kodewil>
	</tujuan>
</barang>

Elemen logbarang memiliki elemen barang dimana didalamnya terdapat element kode, satuan, harga, asal, dan tujuan. Dalam elemen harga terdapat atribut cur = "nmtoken". Dalam elemen asal terdapat elemen pt dan kodewil dan dalam elemen tujuan terdapat elemen pt dan kodewil. Dan ditutup dengan elemen penutup barang.

</logbarang>

Penutup elemen logbarang.

Logbarang.dtd

<?xml encoding="UTF-8"?>
Syntax pada awal dtd.

<!ELEMENTlogbarang (barang)+>
Dalam element dtd logbarang terdapat element dengan nama "barang". Terdapat tanda "+" ini menyatakan bahwa data pada element barang harus ada minimal 1 atau lebih.

<!ATTLISTlogbarang xmlns CDATA#FIXED_''_>
coding diatas : Attlist menyatakan nama element pada xml.

<!ELEMENTbarang (kode?,satuan,harga,asal,tujuan)>
Elemen barang didalamnya terdapat element lain yaitu kode, satuan, harga, asal dan tujuan. Tanda "?" menunjukan bahwa elemen yang memiliki tanda tersebut boleh tidak memiliki data atau bisa memiliki data.

<!ELEMENTkode(#PCDATA)><!ATTLISTkode xmlns CDATA#FIXED_''_>
Elemen kode berisi data atau value. Dengan nama elemen di xml kode.

<!ELEMENTsatuan(#PCDATA)><!ATTLISTsatuan xmlns CDATA#FIXED_''_>
Elemen satuan berisi data atau value. Dengan nama elemen di xml satuan.

<!ELEMENTharga(#PCDATA)><!ATTLISTharga xmlns CDATA#FIXED_''_ cur NMTOKEN#IMPLIED>
Eelemen harga berisi data atau value. Dengan nama elemen di xml harga dan atribut cur dengan nilai nmtoken.

<!ELEMENTasal (pt,kodewil)><!ATTLISTasal xmlns CDATA#FIXED_''_>
Elemen asal didalamnya terdapat elemen pt dan kodewil.

<!ELEMENTtujuan (pt,kodewil)><!ATTLISTtujuan xmlns CDATA#FIXED_''_>
Elemen tujuan didalamnya terdapat elemen pt dan kodewil.

<!ELEMENTpt(#PCDATA)><!ATTLISTpt xmlns CDATA#FIXED_''_>
Elemen pt berisi data atau value. Dengan nama elemen di xml pt.

<!ELEMENTkodewil(#PCDATA)><!ATTLISTkodewil xmlns CDATA#FIXED_''_>
Elemen kodewil berisi data atau value. Dengan nama elemen di xml kodewil.
