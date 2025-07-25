# docker

> Atur kontainer Docker dan image.
> Beberapa subperintah seperti `run` mempunyai dokumentasi terpisah.
> Informasi lebih lanjut: <https://docs.docker.com/reference/cli/docker/>.

- Tampilkan semua daftar kontainer Docker (yang sedang berjalan dan berhenti):

`docker ps {{[-a|--all]}}`

- Nyalakan sebuah kontainer dari citra (image), dengan nama kustom:

`docker run --name {{nama_kontainer}} {{citra}}`

- Nyalakan atau menghentikan kontainer yang tersedia:

`docker {{start|stop}} {{nama_kontainer}}`

- Tarik citra dari registri Docker:

`docker pull {{citra}}`

- Tampilkan daftar citra Docker yang telah diunduh:

`docker images`

- Buka sesi shell didalam sebuah kontainer yang sedang berjalan:

`docker exec {{[-it|--interactive --tty]}} {{nama_kontainer}} {{sh}}`

- Hapus kontainer yang sedang berhenti:

`docker rm {{nama_kontainer}}`

- Ambil dan ikuti semua log dari sebuah kontainer:

`docker logs {{[-f|--follow]}} {{nama_kontainer}}`
