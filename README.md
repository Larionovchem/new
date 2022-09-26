# new
import pygame
from pygame.draw import *

pygame.init()

screen = pygame.display.set_mode((400, 400))


rect (screen, 'blue', (0, 0, 400, 400))
rect (screen, 'green',(0, 200, 400, 400))
circle (screen, 'brown', (100, 100), 25)
circle (screen, 'brown', (200, 200, 50, 120), 25, 30)

pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()