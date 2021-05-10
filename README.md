# 6809
from pygame import *
window = display.set_mode((700, 500))
display.set_caption("Epic cutch-up games")
background = transform.scale(image.load("coridor.png"), (700, 500))
    
            self.image = transform.scale(image.load(player_image), (65,65))
            self.speed = player_speed            
            self.rect = self.image.get_rect()
            self.rect.x = player_x
            self.rect.y = y
        def reset(self):
            window.blit(self.image, (self.rect.x, self.rect.y))
class Player(GameSprite):
    def update(self):
        keys_pressed = key.get_pressed()
        if keys_pressed [K_LEFT]:# and self.rect.x > 5:
            self.rect.x -= self.speed
        if keys_pressed [K_RIGHT]:# and self.rect.x > 5:
            self.rect.x += self.speed
        if keys_pressed [K_UP]:# and self.rect.у > 5:
            self.rect.y -= self.speed
        if keys_pressed [K_DOWN]:# and self.rect.y> 5:
            self.rect.у -= self.speed

    
    
    
    
    display.update()
