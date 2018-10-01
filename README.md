# django-intro-hw1

Create a new route and paste it below. Create a blue-or-red route that takes an argument of blue or red. If it's blue, write "Sky". If it's red, write "Fire". If it's anything else write "ERROR".



urlpatterns = [
    path('<str:entry1>/choice', views.choice, name='choice')
]




def choice(request, entry1):
    if entry1 == "blue":
        print("sky")
    else:
        if entry1 == "red":
            print("fire")
        else:
             print("error")
