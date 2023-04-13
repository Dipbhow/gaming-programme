# gaming-programme
import pygame
pygame.init()

# Set up the window
window_width = 800
window_height = 600
window_title = "My Game"
background_color = (255, 255, 255) # white
game_window = pygame.display.set_mode((window_width, window_height))
pygame.display.set_caption(window_title)

# Main game loop
while True:
    # Handle events
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Draw the background
    game_window.fill(background_color)

    # Update the display
    pygame.display.flip()
