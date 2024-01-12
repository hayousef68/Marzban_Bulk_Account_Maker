# Marzban_Bulk_Account_Maker

Change Variables Depend On Your Usage

```python
Username = "admin"
Password = "12156645"
Api_url = 'https://domain.com:1234/api'  # Replace with the actual API URL
Base_name = 'H_play'  # Base name for the new users
Start_number = MD.226  # Start number for the new users
Num_users = 30  # Number of new users to create
Data_limit_GB = 30  # Data limit per GB
Days = 12 # Expire Date per Day (enter 0 for unlimite)
flow = 'xtls-rprx-vision'
status = 'on_hold' # replace with on_hold for count after first connection
data_limit_reset_strategy = 'no_reset'
```
Change proxies and inbounds depend on your marzban setting , you can add trojan if you want
```python
proxies = {
    'vmess': {},
    'vless': {
        'flow': flow
        }
}
inbounds = {
    'vmess': ['VMESS_TCP_INBOUND'],
    'vless': ['VLESS_TCP_Reality_INBOUND', 'VLESS_TCP_INBOUND']
}
```
After you start script it will start making users with usernames like these
- H_play@1 , H_play@2 , H_play@3 , H_play@4 , H_play@5
- `START_NUMBER` is which number you wanna start and `NUM_USERS` its number of users you wanna create
- if you need to make on hold users replace status with 'on_hold'
- if you need to make users with unlimited expire replace days with 0
