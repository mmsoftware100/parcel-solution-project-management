# Parcel Solution - Project Management 


## Parcel Solution ရေးသားမှု အခြေအနေ 

To track project progress.

## Basic Info


### Wireframe

<img width="4360" alt="shapes at 23-12-26 15 00 22" src="https://github.com/mmsoftware100/parcel-solution-project-management/assets/19356481/93463ba7-3dc8-4332-bd47-260cc1655dc5">


### Basic Data Structure

<img width="864" alt="shapes at 23-12-26 15 20 42" src="https://github.com/mmsoftware100/parcel-solution-project-management/assets/19356481/9eb8fad5-150f-4658-bfe4-de8d69874df4">

### API List
<img width="553" alt="shapes at 23-12-26 15 26 40" src="https://github.com/mmsoftware100/parcel-solution-project-management/assets/19356481/54d88521-ae5e-486a-84f2-c3c680c586d2">


### API Routes


- [POST] /login | phone,password | User
- [GET] /parcels | access_token | [Parcel]
- [POST] /parcels | new_parcel_data | Parcel 
- [DELETE] /parcels/{id} | access_token | Parcel
- [PUT] /parcels/{id} | updated_percel_data | Parcel
- [PUT] /parcel-status | updated_parcel_status_data | Parcel

### JSON Structure

```parcel.json```
```json
{
    "id" : 1,
    "from_user" : {
        "id" : 1,
        "name" : "user name",
        "phone" : "0912345678",
        "email" : "adsfa@email.com"
    },
    "to_user" : {
        "id" : 1,
        "name" : "user name",
        "phone" : "0912345678",
        "email" : "adsfa@email.com"
    },
    "weight" : 1,
    "width" : 1,
    "height" : 1,
    "length" : 1,
    "items" : [
        {
            "id" : 1,
            "name" : "ဂျပ်ဖာ အသေး",
            "unit_price" : 1500.0,
            "quantity" : 1,
            "total_price" : 1500.0
        },
        {
            "id" : 1,
            "name" : "ဖန်ပုလင်း အသေး",
            "unit_price" : 4500.0,
            "quantity" : 2,
            "total_price" : 9000.0
        }
    ],
    "charges" : [
        {
            "id" : 1,
            "charges_id" : 1,
            "priority" : 1,
            "name" : "ခေါက်တို",
            "amount" : 1000,
            "paid" : 0
        },
        {
            "id" : 2,
            "charges_id" : 2,
            "priority" : 2,
            "name" : "ကုန်ကြွေး",
            "amount" : 1000,
            "paid" : 0
        },
        {
            "id" : 3,
            "charges_id" : 3,
            "priority" : 3,
            "name" : "စုစုပေါင်း",
            "amount" : 1000,
            "paid" : 0
        }
    ],
    "delivery_statues" :[
        {
            "id" : 1,
            "gate" : {
                "id" : 1,
                "name" : "Gate One"
            },
            "status" : {
                "id" : 1,
                "name" : "လက်ခံရရှိ"
            },
            "created_at" : "2023-12-26 12:34:56"
        },
        {
            "id" : 2,
            "gate" : {
                "id" : 1,
                "name" : "Gate One"
            },
            "status" : {
                "id" : 1,
                "name" : "တင်ပို့"
            },
            "created_at" : "2023-12-27 05:06:07"
        }
    ],
    "routes" : [
        {
            "id" : 1,
            "gate" :  {
                "id" : 1,
                "name" : "Gate One"
            },
            "gate_type" :  {
                "id" : 1,
                "name" : "ပေးပို့ဂိတ်"
            }
        },
        {
            "id" : 2,
            "gate" :  {
                "id" : 2,
                "name" : "Gate Two"
            },
            "gate_type" :  {
                "id" : 2,
                "name" : "Transit"
            }
        },
        {
            "id" : 3,
            "gate" :  {
                "id" : 3,
                "name" : "Gate Three"
            },
            "gate_type" :  {
                "id" : 3,
                "name" : "Destination"
            }
        }
    ]
}
```
