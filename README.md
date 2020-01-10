# ryu_slg

## Install

```
git clone https://github.com/lagopus/ryu-lagopus-ext
cd ryu-lagopus-ext
git checkout lagopus-general-tunnel-ext
sudo python3 ./setup.py install
cd
git clone https://github.com/hibitomo/ryu_slg
```

## How to use

```
ryu-manager ~/ryu_slg/ryu_slg.py ~/ryu_slg/ryu_slg_init.py
```

## API

```
## Add
curl -X POST -d '{"slice_id":1, "src_ip":"10.0.0.1", "dst_ip":"10.1.0.1", "dst_port":10484}' 127.0.0.1:8080/slice/add
## Delete
curl -X POST -d '{"slice_id":1}' 127.0.0.1:8080/slice/delete
```