- 👋 Hi, I’m @Nayan-cmd21
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Nayan-cmd21/Nayan-cmd21 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
---><!DOCTYPE html>
<html>
<head>
  <title>Maze-Solving Emoji</title>
  <style>
    .maze {
      display: flex;
      flex-wrap: wrap;
      width: 400px;
    }

    .cell {
      box-sizing: border-box;
      width: 20px;
      height: 20px;
      border: 1px solid black;
      background-color: white;
    }

    .emoji {
      font-size: 16px;
      text-align: center;
    }

    .emoji.start {
      background-color: yellow;
    }

    .emoji.finish {
      background-color: green;
    }
  </style>
</head>
<body>
  <div class="maze"></div>

  <script>
    // Define maze dimensions and cell types
    const mazeWidth = 20;
    const mazeHeight = 20;
    const cellTypes = {
      empty: 0,
      wall: 1,
      start: 2,
      finish: 3,
    };

    // Generate a random maze
    const maze = generateMaze(mazeWidth, mazeHeight);
    const mazeElement = document.querySelector('.maze');

    // Display the maze on the page
    maze.forEach(row => {
      row.forEach(cell => {
        const cellElement = document.createElement('div');
        cellElement.classList.add('cell');

        if (cell === cellTypes.wall) {
          cellElement.style.backgroundColor = 'black';
        } else if (cell === cellTypes.start) {
          cellElement.classList.add('emoji', 'start');
          cellElement.textContent = '😊';
        } else if (cell === cellTypes.finish) {
          cellElement.classList.add('emoji', 'finish');
          cellElement.textContent = '🏁';
        }

        mazeElement.appendChild(cellElement);
      });
    });

    // Function to generate a random maze
    function generateMaze(width, height) {
      const maze = [];

      for (let i = 0; i < height; i++) {
        const row = [];

        for (let j = 0; j < width; j++) {
          const cellType = Math.random() > 0.7 ? cellTypes.wall : cellTypes.empty;
          row.push(cellType);
        }

        maze.push(row);
      }

      const startRow = Math.floor(Math.random() * height);
      const startCol = Math.floor(Math.random() * width);
      maze[startRow][startCol] = cellTypes.start;

      const finishRow = Math.floor(height / 2);
      const finishCol = Math.floor(width / 2);
      maze[finishRow][finishCol] = cellTypes.finish;

      return maze;
    }
  </script>
  
  <p>View the code on <a href="https://github.com/your-username/repository-name">GitHub</a>.</p>
</body>
</html>

