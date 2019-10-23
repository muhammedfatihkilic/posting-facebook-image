# posting-facebook-image

import facebook
import pyfacebook
token = "EAAO1vTmPDTkBAAKxsGYIc845GtEcXvz03tWQ1vwPezgZAEZBKwmPAZAxZCQn6IWw2nUDd9gWNd9SXAHyPyVt06fZBNP0nQKkS0KN3ijTRqPHfkXnxFZCjXPFAA4cvr8fWxEQNp2zCFiMKzxno6nxPL4PL4SzH2QARMBJECUZAHWGp7ZAd5ZAZBMHEqFubXB30oo5KD8TFoiK5p3x4Miw3rjcCI"
fb = facebook.GraphAPI(access_token=token)
#fb.put_object(parent_object="me",connection_name="feed",message="hello")

#post_id = "114797233273673"
#profil_id = "102399201180143"
def post_image():
    fb.put_photo(open("test.png",'rb'),message="fatih.")
def delete_post():
    fb.delete_object(profil_id+"_"+post_id)
if __name__ == "__main__":
    post_image()
