# 💾 Amazon EBS Configuration

## Objective

Attach and configure an additional Amazon EBS volume for persistent storage.

---

## Steps Performed

### Create Volume

- Size: 2 GiB
- Type: gp3
- Same Availability Zone as EC2

---

### Attach Volume

Attached the EBS volume to the EC2 instance.

---

### Verify Device

```bash
lsblk
```

---

### Format Volume

```bash
sudo mkfs.ext4 /dev/nvme1n1
```

---

### Create Mount Point

```bash
sudo mkdir /data
```

---

### Mount Volume

```bash
sudo mount /dev/nvme1n1 /data
```

---

### Persistent Mount

Updated:

```
/etc/fstab
```

using the volume UUID.

---

## Verification

```bash
df -h
```

Verified:

```
/data
```

was successfully mounted.

---

## Outcome

Amazon EBS configured successfully with persistent storage across instance reboots.
