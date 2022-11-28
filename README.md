# bigdata
for name, lat, lng ,cnt in zip(df.발생년월일시, df.위도, df.경도 ,df.사망자수):
    folium.Circle([lat, lng], popup=name, radius=cnt*200, color='red',fill_color = 'red').add_to(smap)
CircleMarker 가 아닌 Circle 사용시 m단위로 찍을 수 있음
![캡처](https://user-images.githubusercontent.com/102711363/204182574-4687dbfd-3828-4615-a27e-3120ddc5ea10.PNG)
![2](https://user-images.githubusercontent.com/102711363/204182583-993d59d2-4ead-4dfb-a674-2a9bcccd16be.PNG)

네이버 지도를 이용한 대략적 m 확인
