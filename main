#include "SFML/Graphics.hpp"

int main() {
    sf::RenderWindow renderWindow(sf::VideoMode(256, 256), "render image");

    sf::Event event;
    sf::Texture texture;
    texture.loadFromFile("imagesOutrun/red.png");

    sf::Sprite sprite(texture, sf::IntRect(0, 0, 32, 32));


    while (renderWindow.isOpen()) {
        while (renderWindow.pollEvent(event)) {
            if (event.type == sf::Event::EventType::Closed)
                renderWindow.close();
        }

        renderWindow.clear();
        renderWindow.draw(sprite);
        renderWindow.display();
    }
}
