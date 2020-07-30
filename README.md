![Footloose](https://github.com/mchirico/k8s_the_fun_way/workflows/Footloose/badge.svg)
# k8s_the_fun_way

## Setup footloose

### Step 1
```
curl -Lo footloose https://github.com/weaveworks/footloose/releases/download/0.6.3/footloose-0.6.3-linux-x86_64
chmod +x footloose
sudo mv footloose /usr/local/bin/
```

### Step 2

```
curl -L https://raw.githubusercontent.com/mchirico/k8s_the_fun_way/master/scripts/footloose.yaml -o footloose.yaml
footloose create
footloose ssh root@knode0
```

### Step 3

```
systemctl start docker
```

### Step 4

```
git clone https://github.com/mchirico/kind.git
cd kind
```

### Step 5

```
make cert-manager
```
