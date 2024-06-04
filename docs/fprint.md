## Resources

## Setting up fprint

- To erase the fingerprints for a user run:
```bash
  sudo fprintd-delete "$USER"
```

- To add all fingers to be able to unlock the device run
```bash
  for finger in {left,right}-{thumb,{index,middle,ring,little}-finger}; do sudo fprintd-enroll -f "$finger" "$USER"; done
```

- To verify if your chanegs worked run.
```bash
  fprintd-verify
```



