# HerGPT (Under Early Development)

Love is about the details. By tracking her likes, dislikes, desires, important dates, and other personal facts, you can provide true love like never seen before. The most important thing men fail to do is get data and understand how she feels. With technology, its possible to love like never before.

## Features

- **Likes and Dislikes Table**: Keep a record of her likes and dislikes to help you plan thoughtful surprises, gifts, and activities. Keep track of what her family likes and dislikes aswell.
- **Facts Table**: Store interesting and important facts about her. These can be fundamental truths that are not a like or a dislike
- **Important Dates Table**: Never forget an important date again by keeping track of anniversaries, birthdays, and other significant events.
- **Daily Logs**: A daily log so that the above 3 things can be automatically extracted from it in the future!

## Planned Data Structure

### Likes and Dislikes Table
| Column      | Type    | Description                        |
|-------------|---------|------------------------------------|
| id          | Integer | Primary Key                        |
| type        | String  | 'Like' or 'Dislike'                |
| description | String  | Description of the like or dislike |

### Facts Table
| Column      | Type    | Description             |
|-------------|---------|-------------------------|
| id          | Integer | Primary Key             |
| fact        | String  | A fact about her        |

### Important Dates Table
| Column      | Type    | Description             |
|-------------|---------|-------------------------|
| id          | Integer | Primary Key             |
| date        | Date    | Important date          |
| description | String  | Description of the event|

### Daily Logs Table
| Column      | Type    | Description             |
|-------------|---------|-------------------------|
| id          | Integer | Primary Key             |
| date        | Date    | Important date          |
| description | String  | Description of the day  |

## Planned Tools
The above data can be used
- Logs populator -- Automatically populate the 3 tables based on a daily log entry, increasing effort to reward ratio.
- Gift Generator -- Generate gifts for her and her family based on recent events, like and dislikes.


## Installation

To set up LoveGPT locally:

1. Clone the repository:
    ```sh
    git clone https://github.com/legendarywar/LoveGPT.git
    ```
2. Navigate to the project directory:
    ```sh
    cd LoveGPT
    ```
3. Install the necessary dependencies:
    ```sh
    pip install -r requirements.txt
    ```
4. Run the application:
    ```sh
    chainlit start app.py
    ```

## Usage

- Add new entries to the likes, dislikes, facts, and dates tables through the user interface.
- View and manage the details you've stored about her to ensure you're always attentive and considerate.

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Push your branch and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
